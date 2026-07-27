---
name: Create and capture a booking
description: Place a Headout booking with the idempotent two-step create-then-capture flow.
api: openapi/headout-partner-openapi.yml
operations: [createBooking, updateBooking, getBooking]
---

# Create and capture a Headout booking

Headout bookings are a two-step flow. Never treat step 1 as a confirmed sale.

## Auth
`Headout-Auth: {token}` on every call. `pk_` = live/official bookings; `tk_` =
sandbox testing.

## Steps
1. **Create (step 1)** — `createBooking` (`POST /api/public/v1/booking`) with
   `variantId`, `inventoryId`, `customersDetails`, `variantInputFields`, and
   `price`. The response is a booking in **UNCAPTURED** state. Store its `id`.
2. **Charge your customer** in your own system.
3. **Capture (step 2)** — `updateBooking` (`PUT /api/public/v1/booking/{id}`)
   with `status: PENDING` and your `partnerReferenceId`. This moves the booking
   to **PENDING** and triggers fulfillment.
4. **Verify** — optionally `getBooking` (`GET /booking/{id}`) to read status
   (PENDING → COMPLETED).

## Idempotency & timing
- Capture within **60 minutes** or the booking auto-transitions to
  **CAPTURE_TIMEOUT**.
- Step 2 is retry-safe: on timeout or an ambiguous response, **re-request the
  step-2 capture until you get a success message**. Reuse the same
  `partnerReferenceId` so retries de-duplicate.

## Errors
Envelope: `{ status, error: { code, message } }`. Handle `E_MISSING_PARAMETER`
and `E_INVALID_ARGUMENT` (400) and `E_ERROR_PROCESSING_REQUEST` (500). See
errors/headout-error-codes.yml.

---
name: Browse the catalog and price a variant
description: Find products in a city and pull live availability and pricing for a variant before booking.
api: openapi/headout-partner-openapi.yml
operations: [listProducts, listInventoryByVariant]
---

# Browse the Headout catalog and price a variant

Use the Headout Partner API to discover bookable experiences and get live pricing.

## Auth
Send every request with the `Headout-Auth: {token}` header. Use a `pk_` token in
production and a `tk_` token against `https://sandbox.api.test-headout.com`.

## Steps
1. **List products** — `listProducts` (`GET /api/public/v2/products`) with the
   required `cityCode`. Narrow with `categoryId`, `subCategoryId`, `collectionId`,
   `languageCode` (default `EN`), and `currencyCode`. Page with `offset`/`limit`
   (default 20); follow `nextUrl` / `nextOffset`.
2. **Pick a variant** of the chosen product (a bookable option).
3. **Get inventory & pricing** — `listInventoryByVariant`
   (`GET /api/public/v1/inventory/list-by/variant`) with `variantId`. Optionally
   bound with `startDateTime`/`endDateTime` (`fm-date-time`, ISO 8601 local) and
   set `currencyCode` (ISO 4217). Read `availability` (LIMITED/UNLIMITED/CLOSED),
   `remaining`, and `pricing.persons` / `pricing.groups`.

## Rules
- Enum errors return `E_INVALID_ARGUMENT`; missing required params return
  `E_MISSING_PARAMETER` (see errors/headout-error-codes.yml).
- Only book against inventory whose `availability` is not `CLOSED` and
  `remaining` covers the party size.

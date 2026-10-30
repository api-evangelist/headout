# HeadOut

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Headout is a global experiences marketplace that curates and sells tickets to tours, attractions, events, shows and activities across major cities worldwide. For developers, Headout operates a public Partner API (github.com/headout/api-docs) that lets affiliates and resellers browse the catalog (products, categories, collections and subcategories by city and language), pull live inventory and per-person/per-group pricing for a variant, and place bookings through a two-step create-then-capture flow. The API is versioned by URI path (v1 and v2 under /api/public/), authenticates with a Headout-Auth API key (pk_ production / tk_ sandbox), paginates with offset/limit, and returns a structured error envelope. A registrable seatmap iframe component is offered for seat selection. Headout is backed by 500 Global and Version One Ventures.

**Areas:** Travel · Tours and Activities · Experience · Attractions · Ticketing · Booking · Marketplace · Partner API · Affiliates · Event

## HeadOut on APIs.io

Everything profiled for HeadOut is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/headout/](https://apis.io/providers/headout/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [HeadOut Booking API](https://apis.io/apis/headout/headout-booking-api/) — The Booking API from HeadOut — 2 operation(s) for booking.
- [HeadOut Categories API](https://apis.io/apis/headout/headout-categories-api/) — The Categories API from HeadOut — 1 operation(s) for categories.
- [HeadOut Collections API](https://apis.io/apis/headout/headout-collections-api/) — The Collections API from HeadOut — 1 operation(s) for collections.
- [HeadOut Inventory API](https://apis.io/apis/headout/headout-inventory-api/) — The Inventory API from HeadOut — 1 operation(s) for inventory.
- [HeadOut Products API](https://apis.io/apis/headout/headout-products-api/) — The Products API from HeadOut — 1 operation(s) for products.
- [HeadOut Subcategories API](https://apis.io/apis/headout/headout-subcategories-api/) — The Subcategories API from HeadOut — 1 operation(s) for subcategories.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [headout-partner](https://apis.io/servers/headout/headout-partner/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Headout Agentic Access](https://apis.io/agentic-access/headout/headout-agentic-access/)

#### Collections (6)

Postman and Open Collection request collections.

- [Headout Partner Booking API](https://apis.io/collections/headout/open-headout-booking-api/)
- [Headout Partner Booking Categories API](https://apis.io/collections/headout/open-headout-categories-api/)
- [Headout Partner Booking Collections API](https://apis.io/collections/headout/open-headout-collections-api/)
- [Headout Partner Booking Inventory API](https://apis.io/collections/headout/open-headout-inventory-api/)
- [Headout Partner Booking Products API](https://apis.io/collections/headout/open-headout-products-api/)
- [Headout Partner Booking Subcategories API](https://apis.io/collections/headout/open-headout-subcategories-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Headout Partner Overlay](https://apis.io/overlays/headout/headout-partner-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Headout Authentication](https://apis.io/security/headout/headout-authentication/)
- [Headout Domain Security](https://apis.io/security/headout/headout-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://headout.com)
- [Documentation](https://github.com/headout/api-docs)
- [Getting started](https://github.com/headout/api-docs/wiki/Integration-flow-for-Partners)
- [API reference](https://github.com/headout/api-docs/tree/master/apis)
- [Sign up](https://partner.headout.com/affiliate/)
- [Support](https://www.headout.com/help/)
- [Blog](https://www.headout.com/blog/)
- [Terms of service](https://www.headout.com/terms-of-use/)
- [Privacy policy](https://www.headout.com/privacy-policy/)
- [GitHub](https://github.com/headout)

## API Evangelist rating

**Kin Score 19.0** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 13.7 |
| Contract governance | 4.5 |
| Operational transparency | 10.5 |
| Developer ergonomics | 20.8 |
| Access clarity | 13.2 |

**Agent readiness 24.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/headout/](https://apis.io/providers/headout/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for HeadOut: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/headout/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

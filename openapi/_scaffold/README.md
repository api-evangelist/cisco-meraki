# Quarantined scaffold — not published by Cisco

The OpenAPI documents in this directory were **written by API Evangelist**, modelled from Cisco's
public Meraki documentation. They were never published by Cisco and must not be presented as Cisco
artifacts, cited as evidence of what Cisco ships, or credited in a Kin Score.

They were moved here on **2026-07-31**.

## Why they were quarantined

Cisco publishes the Meraki Dashboard API OpenAPI definition in two places, both live:

> https://github.com/meraki/openapi — `openapi/spec3.json` (OpenAPI 3.0.1)
> https://api.meraki.com/api/v1/openapiSpec (Swagger 2.0, served from the API host)

**670 paths / 957 operations / 411 tags, version 1.72.0.** All 957 operations carry a description
and 879 carry response examples. It is one of the larger and better-maintained public API contracts
in the industry. It is now harvested into `../_original/` and is the only contract this provider
should be scored on.

The document here modelled **24 operations** — about **3%** of what Cisco actually publishes — and
this provider was scoring **29.0 "thin"** as a result. That number was a measurement of API
Evangelist's scaffold, not of Cisco's API.

See `[[scaffold-fabrication-sweep]]` and `[[kin-score-provenance-gap]]` for the general failure mode.

## Contents

`cisco-meraki-openapi.yml` (24 operations, hand-modelled) plus the 8 per-tag files that
`refine-openapis` split out of it.

## Do not

- Restore these to `_original/`.
- Re-run `refine-openapis` against them.
- Point `apis.yml` at them.

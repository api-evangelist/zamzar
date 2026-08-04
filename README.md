# Zamzar

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Zamzar is an online file conversion platform with a REST API for converting files between 100+ formats including documents, videos, audio, images, and CAD files. The API supports over 1,100 distinct format conversions processed asynchronously using a credit-based billing model.

## Developer Resources

- **Developer Portal:** https://developers.zamzar.com/
- **API Documentation:** https://developers.zamzar.com/docs
- **OpenAPI Specification:** https://github.com/zamzar/zamzar-spec
- **GitHub Organization:** https://github.com/zamzar
- **Pricing:** https://developers.zamzar.com/pricing
- **Status Page:** https://www.zamzarstatus.com/
- **Blog:** https://blog.zamzar.com/

## API Overview

The Zamzar API is a REST API using HTTP Basic Auth (API key as username). It provides two environments:

- **Production:** `https://api.zamzar.com/v1/`
- **Sandbox:** `https://sandbox.zamzar.com/v1/`

### Key Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/formats/` | GET | List all supported formats |
| `/formats/{format}` | GET | Get details for a specific format |
| `/jobs` | POST | Create a conversion job |
| `/jobs/{id}` | GET | Check conversion job status |
| `/files/{id}/content` | GET | Download converted file |
| `/files/{id}` | DELETE | Delete a file from Zamzar servers |

### SDKs

- **Python:** https://github.com/zamzar/zamzar-python
- **PHP:** https://github.com/zamzar/zamzar-php
- **Java:** https://github.com/zamzar/zamzar-java

## Catalog Files

- [`apis.yml`](apis.yml) — APIs.json 0.19 provider profile
- [`plans/zamzar-plans-pricing.yml`](plans/zamzar-plans-pricing.yml) — Pricing plans and tiers
- [`rate-limits/zamzar-rate-limits.yml`](rate-limits/zamzar-rate-limits.yml) — API rate limits
- [`finops/zamzar-finops.yml`](finops/zamzar-finops.yml) — Financial operations guidance

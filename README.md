# Zamzar

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

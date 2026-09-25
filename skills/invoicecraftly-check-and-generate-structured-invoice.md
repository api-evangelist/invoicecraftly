---
name: invoicecraftly-check-and-generate-structured-invoice
description: Check EN16931-core readiness of an invoice and then generate the structured EN16931-core XML document.
api: openapi/invoicecraftly-openapi.json
operations:
- checkInvoiceReadiness
- generateStructuredInvoice
generated: '2026-09-25'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/invoicecraftly-openapi.json ; every operationId checked against the contract
---

# invoicecraftly-check-and-generate-structured-invoice

Check EN16931-core readiness of an invoice and then generate the structured EN16931-core XML document.

## Steps

1. 1. Call `checkInvoiceReadiness` (POST /api/v1/invoices/readiness) – requires the Bearer authentication header.
2. 2. Call `generateStructuredInvoice` (POST /api/v1/documents/structured) – requires the Bearer authentication header.

## Rules

- Authentication: Include an `Authorization: Bearer <token>` header for all requests.

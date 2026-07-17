# Affinity Health

Affinity provides infrastructure for software platforms connecting healthcare practices to a
network of compounding pharmacies.

This organization is the home of Affinity's public API contract, official server-side SDKs, and
integration starters.

## Developer projects

- [TypeScript SDK](https://github.com/affinity-health/affinity-typescript)
- [Python SDK](https://github.com/affinity-health/affinity-python)
- [Go SDK](https://github.com/affinity-health/affinity-go)
- [Java SDK](https://github.com/affinity-health/affinity-java)
- [OpenAPI specification](https://github.com/affinity-health/affinity-openapi)
- [SST backend starter](https://github.com/affinity-health/affinity-sst-backend)

The public developer projects are currently being prepared for their first release. Package names,
versions, and API stability guarantees will be documented before publication.

## Product language

- A **provider** is an individual clinician or prescriber.
- A **practice** is the customer organization and API tenant.
- A **location** is a physical practice site.

Affinity SDKs are designed for trusted server environments. Never expose an Affinity API key in a
browser, mobile application, public repository, or client-visible log.


# Affinity Health

Affinity connects software platforms and healthcare practices to a network of compounding
pharmacies. One API request creates, signs and sends a prescription order; Affinity tracks it
until delivery.

## Developers

- **API documentation:** [docs.affinityrx.com](https://docs.affinityrx.com)
- **API contract:** [api.affinityrx.com/v1/openapi.json](https://api.affinityrx.com/v1/openapi.json).
  The current `Affinity-Version` is `2026-10-28`.
- Use a Test key while you build. Test orders go to a test pharmacy.

## Official SDKs

Each SDK is generated from the API contract with [Fern](https://buildwithfern.com).

| Language | Repository | Install |
| --- | --- | --- |
| TypeScript | [affinity-typescript](https://github.com/affinity-health/affinity-typescript) | `npm install @affinity-health/sdk@next` |
| Python | [affinity-python](https://github.com/affinity-health/affinity-python) | From GitHub, tag `v0.4.0` |
| Go | [affinity-go](https://github.com/affinity-health/affinity-go) | `go get github.com/affinity-health/affinity-go@v0.4.1` |
| Java | [affinity-java](https://github.com/affinity-health/affinity-java) | From GitHub, tag `v0.4.0` |
| C# | [affinity-csharp](https://github.com/affinity-health/affinity-csharp) | From GitHub, tag `v0.4.0` |

The TypeScript SDK is a beta on npm's `next` tag. The other SDKs are not on a package registry yet;
each README shows how to install from GitHub. More about the contract:
[affinity-openapi](https://github.com/affinity-health/affinity-openapi).

Every write takes an idempotency key. Save it with the order before you send it, and send the same
key when you retry, so a retry never creates a second order.

## Terms

- A **provider** is an individual clinician or prescriber.
- A **practice** is the customer organization and API tenant.

The SDKs are for trusted servers. Never put an Affinity API key in a browser, a mobile
application, a public repository or a log.

## Security

Report a vulnerability to `support@affinityrx.com` with "Security" in the subject. Do not open a
public issue.

# Sequin (sequin-io)

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

Sequin is an open-source Postgres change data capture (CDC) engine that streams Postgres rows and changes to streams, queues, and search indexes - Kafka, SQS, SNS, Kinesis, Redis, NATS, RabbitMQ, Elasticsearch, Typesense, GCP Pub/Sub, Azure Event Hubs, and HTTP/webhook endpoints - with exactly-once processing, backfills, and low-latency delivery. Sequin is self-hostable (MIT) and also available as Sequin Cloud. Resources are configured declaratively via a `sequin.yaml` file or programmatically through the Management API; consumers can pull changes over HTTP via the Sequin Stream sink.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/apis.yml)

## Tags

- Change Data Capture
- CDC
- Postgres
- Streaming
- Open Source
- Data Pipeline

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Sequin Sink Consumers API

Programmatically create, list, get, update, and delete sink consumers - the destinations that stream Postgres changes to Kafka, SQS, Redis, HTTP endpoints, and other targets. Mirrors the declarative sink definitions in `sequin.yaml`.

- **Human URL:** [https://sequinstream.com/docs/management-api/sink-consumers/list](https://sequinstream.com/docs/management-api/sink-consumers/list)
- **Base URL:** `https://api.sequinstream.com/api`

#### Tags

- Sinks
- Consumers
- CDC

#### Properties

- [Documentation](https://sequinstream.com/docs/management-api/introduction)
- [API Reference](https://sequinstream.com/docs/management-api/sink-consumers/list)
- [OpenAPI](openapi/sequin-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sequin-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sequin-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sequin Postgres Databases API

Manage the source Postgres database connections Sequin replicates from - create, list, get, update, and delete connections, test connectivity and permissions, and refresh the cached table schema.

- **Human URL:** [https://sequinstream.com/docs/management-api/postgres_databases/list](https://sequinstream.com/docs/management-api/postgres_databases/list)
- **Base URL:** `https://api.sequinstream.com/api`

#### Tags

- Postgres
- Databases
- Sources

#### Properties

- [API Reference](https://sequinstream.com/docs/management-api/postgres_databases/list)
- [OpenAPI](openapi/sequin-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sequin-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sequin-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sequin HTTP Endpoints API

Manage reusable HTTP endpoint destinations used by webhook sinks - create, list, get, update, and delete the base URLs, headers, and encrypted headers that Sequin posts change events to.

- **Human URL:** [https://sequinstream.com/docs/management-api/http-endpoints/get](https://sequinstream.com/docs/management-api/http-endpoints/get)
- **Base URL:** `https://api.sequinstream.com/api`

#### Tags

- HTTP Endpoints
- Webhooks
- Destinations

#### Properties

- [API Reference](https://sequinstream.com/docs/management-api/http-endpoints/get)
- [OpenAPI](openapi/sequin-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sequin-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sequin-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sequin Backfills API

Trigger and manage backfills for a sink - replay existing Postgres rows (full or partial) into a destination at any point in time. Create, list, get, update, and delete backfills scoped to a given sink.

- **Human URL:** [https://sequinstream.com/docs/management-api/backfills/create](https://sequinstream.com/docs/management-api/backfills/create)
- **Base URL:** `https://api.sequinstream.com/api`

#### Tags

- Backfills
- Replay
- CDC

#### Properties

- [API Reference](https://sequinstream.com/docs/management-api/backfills/create)
- [OpenAPI](openapi/sequin-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sequin-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sequin-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sequin Stream Pull API

HTTP pull consumption surface for the Sequin Stream sink. Consumers receive batches of change messages, then acknowledge (ack) or negatively acknowledge (nack) them, giving at-least-once / exactly-once processing without an external broker.

- **Human URL:** [https://sequinstream.com/docs/reference/sinks/sequin-stream](https://sequinstream.com/docs/reference/sinks/sequin-stream)
- **Base URL:** `https://api.sequinstream.com/api`

#### Tags

- Consumption
- HTTP Pull
- Exactly Once

#### Properties

- [Documentation](https://sequinstream.com/docs/reference/sinks/sequin-stream)
- [OpenAPI](openapi/sequin-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sequin-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sequin-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/sequinstream)
- [LinkedIn](https://www.linkedin.com/company/sequin-io)
- [Website](https://sequinstream.com)
- [Documentation](https://sequinstream.com/docs)
- [Plans](plans/sequin-io-plans-pricing.yml)
- [Rate Limits](rate-limits/sequin-io-rate-limits.yml)
- [Fin Ops](finops/sequin-io-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

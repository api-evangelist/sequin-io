# Sequin (sequin-io)

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

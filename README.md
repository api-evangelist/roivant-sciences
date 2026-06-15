# Roivant Sciences (roivant-sciences)

Roivant Sciences (Nasdaq: ROIV) is a holding company that builds focused subsidiary
biotech and health-tech operating units called "Vants." Founded by Vivek Ramaswamy
in 2014 and now led by CEO Matt Gline, Roivant has launched companies across
immunology (Immunovant, Priovant, Covant, PsiThera), pulmonology (Pulmovant),
delivery technology (Genevant, Proxima), virtual care (Zest Health), and
health-data infrastructure (Datavant, Lokavant). Roivant's most material technology
surface is operated by Datavant — the US health-data exchange and tokenization
network it co-founded — which connects 80,000+ hospitals and clinics, links data
for 100% of US payers, and operates a public EHR data-extraction API under the
Healthjump brand. Lokavant operates a customer-only Clinical Trial Intelligence
Platform on AWS. The drug-discovery Vants (Immunovant, Priovant, Genevant, etc.)
do not expose developer APIs.

**APIs.json:** [https://github.com/api-evangelist/roivant-sciences](https://github.com/api-evangelist/roivant-sciences)

## Scope

- **Type:** Index
- **Access:** 3rd-Party

## Tags

- Biotech
- Pharmaceutical
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Datavant Healthjump EHR Integration API

Public REST API operated by Datavant (via the acquired Healthjump platform) for
extracting clinical and financial data from 70+ on-premise and cloud-hosted
ambulatory EHR/PM systems. Datavant standardizes 300+ data elements across the
connected systems and delivers them via API, webhooks, flat file, or HL7. The
API surface is published at apidocs.healthjump.com and serves customers building
patient engagement, quality reporting, and population-health products on top of
ambulatory EHR data.

- **Human URL:** [https://www.datavant.com/products/ehr-integrations](https://www.datavant.com/products/ehr-integrations)
- **Base URL:** `https://api.healthjump.com`

#### Tags

- Electronic Health Records
- Health Data
- Integration
- EHR
- Interoperability
- Datavant
- Healthjump

#### Properties

- [Documentation](https://apidocs.healthjump.com)
- [API Reference](https://apidocs.healthjump.com)
- [Getting Started](https://api.healthjump.com)
- [Developer Portal](https://apidocs.healthjump.com)
- [Portal](https://portal.datavant.com)
- [Support](https://support.healthjump.com)
- [Integrations](https://www.datavant.com/products/ehr-integrations)
- [Status Page](https://status.datavant.com)
- [OpenAPI](openapi/datavant-healthjump-ehr-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datavant-healthjump-ehr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datavant-healthjump-ehr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/datavant-healthjump-patient-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/datavant-healthjump-encounter-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/datavant-healthjump-vitals-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Spectral Rules](rules/datavant-healthjump-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

### Datavant Tokenization (Datavant Connect)

Datavant's privacy-preserving tokenization technology lets organizations link
patient records across datasets without exchanging personally identifiable
information. It is delivered as a downloadable Datavant CLI (Mac/Windows/Linux)
plus a Datavant Desktop GUI, runnable on-premise or in the customer's cloud
environment, with companion documentation in the Datavant Help Center. The
tokenization layer powers the broader Datavant Connect platform (Linkage
Solutions, Privacy Solutions, Retrieval Solutions) and the Switchboard-style
data ecosystem that brokers exchange across payers, providers, and 350+
real-world data partners.

- **Human URL:** [https://www.datavant.com/products/connect-linkage](https://www.datavant.com/products/connect-linkage)
- **Base URL:** `https://portal.datavant.com`

#### Tags

- Tokenization
- Privacy
- Patient Linkage
- Health Data
- Real World Data
- Datavant
- CLI

#### Properties

- [Documentation](https://datavant-aws-marketplace-files.s3.amazonaws.com/tokenization_user_guide.pdf)
- [C L I](https://portal.datavant.com)
- [Portal](https://portal.datavant.com)
- [Status Page](https://status.datavant.com)
- [Marketplace](https://www.datavant.com/partnerships/cloud-integrations)
- [White Paper](https://www.datavant.com/white-papers/datavant-connect-overview-tokenization-technology-structured-data)
- [Postman Collection](collections/datavant-healthjump-ehr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datavant-healthjump-ehr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lokavant Clinical Trial Intelligence Platform

Lokavant is Roivant's clinical-trial intelligence operating unit. Its platform
ingests data via 21+ source connectors and a proprietary repository of 2,000+
harmonized prior trials plus 14,000+ third-party trials, surfacing predictive
analytics for sponsors and CROs through two named products: Oversight
(risk-based quality management at study/country/site/patient level) and Insight
(performance benchmarking against the historical trial corpus). The platform
runs on AWS — Amazon Cognito for authentication with customer SAML2/OIDC SSO,
API Gateway + Lambda for composite services, ECS/Fargate microservices,
Snowflake data marts, and Apache Airflow for ingestion. Access is invite-only
for sponsor/CRO customers; there is no public developer portal or OpenAPI spec.

- **Human URL:** [https://www.lokavant.com](https://www.lokavant.com)
- **Base URL:** `https://www.lokavant.com`

#### Tags

- Clinical Trials
- Clinical Trial Intelligence
- Predictive Analytics
- Risk-Based Monitoring
- Trial Forecasting
- Lokavant
- Customer Only

#### Properties

- [Portal](https://www.lokavant.com)
- [Documentation](https://aws.amazon.com/startups/learn/lokavant-a-paradigm-shift-in-clinical-trial-intelligence-through-aws-partnership)
- [Blog](https://blog.lokavant.com)
- [Postman Collection](collections/datavant-healthjump-ehr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datavant-healthjump-ehr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Datavant Connect Customer Portal

Datavant Connect is the customer-facing portal that brokers access to
Datavant's linkage, privacy, and retrieval solutions. Access is invite-only
and requires portal-administrator credentials; the portal also fronts the
Aetion Evidence Platform (acquired by Datavant in 2024) for real-world
evidence workflows. Public API documentation for Connect itself is not
published — partners integrate through the Datavant CLI for tokenization
and through the Healthjump API for EHR extraction.

- **Human URL:** [https://portal.datavant.com](https://portal.datavant.com)
- **Base URL:** `https://portal.datavant.com`

#### Tags

- Health Data
- Real World Evidence
- Data Exchange
- Datavant
- Aetion
- Customer Only

#### Properties

- [Portal](https://portal.datavant.com)
- [Documentation](https://www.datavant.com/products/connect-linkage)
- [Status Page](https://status.datavant.com)
- [Postman Collection](collections/datavant-healthjump-ehr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datavant-healthjump-ehr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://roivant.com)
- [Documentation](https://roivant.com/companies)
- [Blog](https://roivant.com/news/)
- [Investor Relations](https://investor.roivant.com)
- [GitHub Organization](https://github.com/datavant)
- [LinkedIn](https://www.linkedin.com/company/roivant-sciences)
- [Terms of Service](https://roivant.com/terms-of-use/)
- [Privacy Policy](https://roivant.com/privacy-policy/)
- [Plans](plans/roivant-sciences-plans-pricing.yml)
- [Rate Limits](rate-limits/roivant-sciences-rate-limits.yml)
- [Fin Ops](finops/roivant-sciences-finops.yml)
- [Vocabulary](vocabulary/roivant-sciences-vocabulary.yml)
- [JSON-LD](json-ld/roivant-sciences-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com

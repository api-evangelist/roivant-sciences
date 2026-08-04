# Roivant Sciences (roivant-sciences)

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

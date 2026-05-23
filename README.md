# Roivant Sciences

Roivant Sciences (Nasdaq: **ROIV**) is a New York-headquartered biotech holding
company founded by Vivek Ramaswamy in 2014 and now led by CEO **Matt Gline**.
Roivant builds focused operating subsidiaries called **Vants** that span
drug discovery, drug delivery, virtual care, and health-data infrastructure.

This repository is the API Evangelist profile of Roivant's API surface area.
The drug-discovery Vants do not expose developer APIs; the material technology
surface is operated by **Datavant** (US health-data exchange and tokenization
network) and **Lokavant** (clinical-trial intelligence platform).

> "Reinventing the discovery, development, and commercialization of new medicines."
> — Roivant.com

## Vant landscape

### Biopharma Vants (no developer APIs)
- **[Immunovant](https://www.immunovant.com)** — anti-FcRn antibodies for autoimmune disease
- **[Priovant](https://www.priovanttx.com)** — targeted autoimmune therapies (brepocitinib franchise)
- **[Covant](https://www.covanttx.com)** — oral and long-acting injectable FcRn inhibitors
- **[Genevant](https://www.genevant.com)** — LNP and ligand-conjugate delivery for RNA/gene editing (700+ patents)
- **[Pulmovant](https://www.pulmovant.com)** — inhaled pulmonary therapeutics (mosliciguat)
- **[PsiThera](https://psithera.com)** — oral small-molecule immunology (sTNFα, TL1A)
- **[Proxima](https://proximabio.com)** — proximity therapeutics platform
- **[Zest Health](https://www.zesthealth.com)** — virtual dermatology clinic (psoriasis, eczema)

### Tech / Data Vants (this profile's focus)
- **[Datavant](https://www.datavant.com)** — US health-data exchange, tokenization, EHR integration; acquired Ciox (2021) and Aetion (2024)
- **[Lokavant](https://www.lokavant.com)** — clinical-trial intelligence platform for sponsors and CROs

### Divested
- **Telavant** sold to Roche for $7.1B upfront + $150M milestone (Dec 2023)
- **Myovant, Urovant, Enzyvant, Altavant, Spirovant** transferred to Sumitomo Dainippon Pharma in the Dec 2019 Sumitovant Biopharma transaction

## Documented APIs

| API | Status | Auth | Public docs |
|---|---|---|---|
| [Datavant Healthjump EHR Integration API](openapi/datavant-healthjump-ehr-openapi.yml) | Production | OAuth2 client credentials | [apidocs.healthjump.com](https://apidocs.healthjump.com) |
| Datavant Tokenization (CLI) | Production | On-prem / customer cloud | [Tokenization User Guide (PDF)](https://datavant-aws-marketplace-files.s3.amazonaws.com/tokenization_user_guide.pdf) |
| Lokavant Clinical Trial Intelligence Platform | Customer-only | Cognito + SAML2/OIDC SSO | [AWS case study](https://aws.amazon.com/startups/learn/lokavant-a-paradigm-shift-in-clinical-trial-intelligence-through-aws-partnership) |
| Datavant Connect Customer Portal | Customer-only | Portal-admin invite | [portal.datavant.com](https://portal.datavant.com) |

### Datavant scale
- 60+ million healthcare records moved
- 80,000+ hospitals and clinics connected
- 75% of the top 100 largest US health systems
- 100% of US payers reached (direct or via health systems)
- 350+ real-world data partners
- 20 of top 20 life-sciences companies
- 70+ ambulatory EHR/PM systems connected via Healthjump (Allscripts, Athenahealth, Aprima, Centricity, eClinicalWorks, Elation Health, Epic, Greenway Intergy / PrimeSUITE, MEDITECH, NextGen, Practice Fusion, MacPractice, etc.)
- ~300 standardized clinical and financial data elements

### Lokavant scale
- 21+ source connectors into the Clinical Data Hub
- 2,000+ harmonized prior trials in the proprietary repository
- 14,000+ third-party trials referenced
- Architecture: Amazon Cognito SSO (SAML2/OIDC), API Gateway + Lambda, ECS/Fargate microservices, Snowflake data marts, AWS Managed Apache Airflow ingestion, CloudFront global distribution
- Products: **Oversight** (risk-based monitoring), **Insight** (benchmarking), **Spectrum v15** (forecasting), **Feasibility AI**, **Medical Monitoring**

## Repository layout

```
roivant-sciences/
├── apis.yml                              # APIs.yml index of all surfaces
├── README.md                             # This file
├── openapi/
│   └── datavant-healthjump-ehr-openapi.yml
├── json-schema/
│   ├── datavant-healthjump-patient-schema.json
│   ├── datavant-healthjump-encounter-schema.json
│   └── datavant-healthjump-vitals-schema.json
├── json-structure/
│   └── datavant-healthjump-structure.json
├── json-ld/
│   └── roivant-sciences-context.jsonld
├── examples/
│   ├── datavant-healthjump-patient-example.json
│   ├── datavant-healthjump-encounter-example.json
│   └── datavant-healthjump-vitals-example.json
├── rules/
│   └── datavant-healthjump-rules.yml      # Spectral ruleset
├── capabilities/
│   ├── health-data-network.yaml           # Composed workflow
│   └── shared/
│       ├── datavant-healthjump-ehr.yaml
│       └── lokavant-clinical-trial-intelligence.yaml
├── vocabulary/
│   └── roivant-sciences-vocabulary.yml
├── plans/
│   └── roivant-sciences-plans-pricing.yml
├── rate-limits/
│   └── roivant-sciences-rate-limits.yml
└── finops/
    └── roivant-sciences-finops.yml
```

## Notable absences

- **No public OpenAPI / Swagger / Postman exports.** The Healthjump API exists at `apidocs.healthjump.com` but its content is gated behind navigation that 404s to crawlers; the OpenAPI in this repo is a reconstructed sketch from the Datavant product page and the public Healthjump support knowledge base.
- **No public GitHub repos for Datavant** (org exists with 119 followers, zero public repos). **No public GitHub org for Roivant, Lokavant, Immunovant, Genevant, Priovant, Covant, Pulmovant, PsiThera, Proxima.** The GitHub org named `roivant` belongs to Sumitovant Digital Innovation and is dormant.
- **No public pricing** for Datavant or Lokavant — both are enterprise-sales motions.
- **No public rate-limit documentation** for the Healthjump API.
- **No status page for Healthjump or Lokavant** — only `status.datavant.com` covers two components (Portal, Datavant CLI).
- **No SDKs** advertised by Datavant or Lokavant beyond the Datavant CLI / Datavant Desktop GUI.

## Sources

- https://roivant.com
- https://www.roivant.com/companies
- https://en.wikipedia.org/wiki/Roivant_Sciences
- https://www.datavant.com
- https://www.datavant.com/about
- https://www.datavant.com/products/ehr-integrations
- https://www.datavant.com/solutions/health-data-extraction
- https://www.datavant.com/electronic-health-records/the-story-of-healthjump
- https://apidocs.healthjump.com
- https://api.healthjump.com
- https://support.healthjump.com
- https://portal.datavant.com
- https://status.datavant.com
- https://www.lokavant.com
- https://aws.amazon.com/startups/learn/lokavant-a-paradigm-shift-in-clinical-trial-intelligence-through-aws-partnership
- https://github.com/datavant

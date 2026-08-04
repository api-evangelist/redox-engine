# Redox (redox-engine)

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

Redox is a healthcare interoperability platform that lets digital health vendors, providers, and payers send, receive, process, and act on healthcare data at scale. Redox sits between digital health applications and the broader healthcare ecosystem, normalizing data across HL7v2, CDA, X12, DICOM, and HL7 FHIR R4, with 100+ EHR connections (Epic, Oracle Health/Cerner, MEDITECH, Athenahealth, eClinicalWorks, NextGen, Allscripts/Veradigm, etc.) and onramps into clinical networks like Carequality, CommonWell, TEFCA, and DirectTrust. Redox exposes three primary APIs — the FHIR R4 API, the Redox Data Model API (proprietary JSON event types), and the Platform API for managing organization configuration — secured with OAuth 2.0 and user-level API keys, and operates HITRUST r2 / SOC 2 Type 2 certified infrastructure processing 20B+ healthcare transactions a year across 12,200+ connected organizations.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/redox-engine/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Healthcare, Healthcare Interoperability, EHR, Electronic Health Records, FHIR, HL7, HL7v2, R4, SMART on FHIR, CDA, DICOM, Digital Health, Patient Data, Providers, Payers, Data Model API, Platform API, Integration Platform, OAuth 2.0, Carequality, CommonWell, TEFCA, EMPI, Bulk Data

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Redox FHIR R4 API

OAuth 2.0-secured HL7 FHIR R4 surface for notifications, queries, and writeback messages between Redox-connected systems, templated per destination and environment.

**Human URL:** [https://docs.redoxengine.com/api-reference/fhir-api-reference/](https://docs.redoxengine.com/api-reference/fhir-api-reference/)

**Base URL:** `https://api.redoxengine.com/fhir/R4/{destination-slug}/{environment-type}`

#### Tags
- FHIR, R4, HL7, Healthcare, Patient Access, Notifications, Queries, Writebacks, USCDI

#### Properties
- [Documentation](https://docs.redoxengine.com/api-reference/fhir-api-reference/)
- [APIReference](https://docs.redoxengine.com/api-reference/fhir-api-reference/)
- [Authentication](https://docs.redoxengine.com/api-reference/redox-data-model-api/authenticate-an-oauth-api-key/)
- [Errors](https://docs.redoxengine.com/api-reference/error-handling-and-responses/)
- [RateLimits](https://docs.redoxengine.com/api-reference/quotas-and-constraints/)

### Redox Data Model API

Redox's proprietary JSON event-type API (PatientAdmin, ClinicalSummary, Orders, Results, Scheduling, Notes, Media, PatientSearch, Provider, etc.) covering notifications, queries, and writebacks across all connected systems.

**Human URL:** [https://docs.redoxengine.com/api-reference/redox-data-model-api/](https://docs.redoxengine.com/api-reference/redox-data-model-api/)

**Base URL:** `https://api.redoxengine.com/endpoint`

#### Tags
- Data Model, JSON, Healthcare, Clinical Data, Notifications, Queries, Orders, Results, Scheduling

#### Properties
- [Documentation](https://docs.redoxengine.com/api-reference/redox-data-model-api/)
- [APIReference](https://docs.redoxengine.com/api-reference/redox-data-model-api/)
- [Authentication](https://docs.redoxengine.com/api-reference/redox-data-model-api/authenticate-an-oauth-api-key/)
- [Errors](https://docs.redoxengine.com/api-reference/error-handling-and-responses/)
- [RateLimits](https://docs.redoxengine.com/api-reference/quotas-and-constraints/)

### Redox Platform API

Management API for Redox organization configuration: access control, alerts, audit events, configs, config modifiers, credentials, destinations, environments, filters, logs, OAuth API keys, promotions, sources, subscriptions, translation sets, and VPNs.

**Human URL:** [https://docs.redoxengine.com/api-reference/platform-api/](https://docs.redoxengine.com/api-reference/platform-api/)

**Base URL:** `https://api.redoxengine.com/platform`

#### Tags
- Management, Configuration, Sources, Destinations, Subscriptions, Filters, Translation Sets, Environments, Audit Events, Connections

#### Properties
- [Documentation](https://docs.redoxengine.com/api-reference/platform-api/)
- [APIReference](https://docs.redoxengine.com/api-reference/platform-api/)
- [Authentication](https://docs.redoxengine.com/api-reference/platform-api/authenticate-a-user-level-api-key/)
- [Errors](https://docs.redoxengine.com/api-reference/error-handling-and-responses/)
- [RateLimits](https://docs.redoxengine.com/api-reference/quotas-and-constraints/)

### Redox HL7 v2 Library

Open-source JavaScript library for parsing and generating HL7 v2 messages, maintained by Redox on GitHub.

**Human URL:** [https://github.com/RedoxEngine/redox-hl7-v2](https://github.com/RedoxEngine/redox-hl7-v2)

#### Tags
- HL7, HL7v2, Parser, JavaScript, Open Source

#### Properties
- [GitHubRepository](https://github.com/RedoxEngine/redox-hl7-v2)
- [SDK](https://github.com/RedoxEngine/redox-hl7-v2)

## Common Properties

- [Website](https://www.redoxengine.com)
- [DeveloperPortal](https://developer.redoxengine.com)
- [Documentation](https://docs.redoxengine.com)
- [APIReference](https://docs.redoxengine.com/api-reference/)
- [Quickstart](https://docs.redoxengine.com/quickstart-for-redox/)
- [GettingStarted](https://docs.redoxengine.com/basics/what-is-redox/)
- [Authentication](https://docs.redoxengine.com/api-reference/redox-data-model-api/authenticate-an-oauth-api-key/)
- [Console](https://dashboard.redoxengine.com)
- [Sandbox](https://docs.redoxengine.com/quickstart-for-redox/)
- [Pricing](https://www.redoxengine.com/contact/)
- [SignUp](https://www.redoxengine.com/contact/)
- [Support](https://docs.redoxengine.com/troubleshooting/)
- [StatusPage](https://status.redoxengine.com)
- [ChangeLog](https://docs.redoxengine.com/product-changelog/)
- [Security](https://docs.redoxengine.com/security/)
- [Compliance](https://www.redoxengine.com/trust/)
- [Blog](https://www.redoxengine.com/blog/)
- [Customers](https://www.redoxengine.com/customers/)
- [Partners](https://www.redoxengine.com/partners/)
- [LinkedIn](https://www.linkedin.com/company/redox-inc-)
- [X](https://x.com/RedoxEngine)
- [YouTube](https://www.youtube.com/c/RedoxEngine)
- [GitHubOrganization](https://github.com/RedoxEngine)

## Features

- **Healthcare Data Normalization** — Universal translation across HL7v2, CDA, X12, DICOM, and HL7 FHIR R4.
- **100+ EHR Connections** — Pre-built connectivity to Epic, Oracle Health/Cerner, MEDITECH, Athenahealth, eClinicalWorks, NextGen, Allscripts/Veradigm, and more.
- **Clinical Network Onramps** — Integrated access to Carequality, CommonWell, TEFCA, and DirectTrust.
- **Patient Identity (EMPI)** — Redox EMPI powered by Verato for record linkage.
- **Cloud Connectivity** — Onramps into AWS, Azure, GCP, Databricks, and Snowflake.
- **Data Operations** — Filters, translation sets, and config modifiers for customizing processing.
- **Subscriptions and Orchestration** — Event subscriptions and conditional routing.
- **Bulk and Real-Time Delivery** — Real-time, bulk, and batch delivery modes.
- **Environments and Promotions** — Dev/staging/prod with promotion workflows.
- **HITRUST and SOC 2** — HITRUST r2 certified and SOC 2 Type 2 compliant.

## Use Cases

- Digital Health EHR Integration
- Patient Access and Engagement
- Care Coordination and Discharge
- Population Health and Registries
- Payer Data Exchange (HEDIS, Prior Auth)
- Lab Order and Result Routing
- Medical Device Data Capture
- EHR Migration and Conversion
- Life Sciences Real-World Data
- Cloud Data Warehouse Hydration (Snowflake, Databricks, BigQuery, S3, Azure)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com

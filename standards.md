# Standards & API Reference

> Project: Vendor Discovery & Vetting · Generated: 2026-05-07

## Industry Standards & Specifications

### ISO Standards

- **ISO 9001:2015 — Quality Management Systems**
  https://www.iso.org/standard/62085.html
  Baseline certification for supplier qualification; most vendor discovery platforms use ISO 9001 as a minimum filter criterion when evaluating supplier quality.

- **ISO 14001:2015 — Environmental Management Systems**
  https://www.iso.org/standard/60857.html
  Increasingly included in supplier ESG evaluation scorecards; relevant for sustainability-focused vendor vetting and environmental compliance tracking.

- **ISO 27001:2022 — Information Security Management Systems**
  https://www.iso.org/standard/27001
  Control 5.21 specifically addresses managing information security risks in the ICT supply chain. Critical for vetting SaaS and technology vendors.

- **ISO 20400:2017 — Sustainable Procurement Guidance**
  https://www.iso.org/standard/63026.html
  Provides a framework for integrating sustainability into every stage of the procurement cycle, from policy development and risk assessment to supplier selection and performance monitoring.

- **ISO 44001:2017 — Collaborative Business Relationship Management Systems**
  https://www.iso.org/standard/72798.html
  Defines requirements for establishing and managing collaborative business relationships, complementing procurement standards with guidance on buyer-supplier partnership management.

- **ISO/IEC 19845:2015 — Universal Business Language (UBL) 2.1**
  https://www.iso.org/standard/66370.html
  International standard for electronic business documents including purchase orders, invoices, and procurement documents. Foundation for PEPPOL and cross-border e-procurement.

### W3C & IETF Standards

- **RFC 6749 — OAuth 2.0 Authorization Framework**
  https://datatracker.ietf.org/doc/html/rfc6749
  Industry-standard protocol for API authorization. Used by procurement platforms (Coupa, SAP Ariba) for secure third-party API access and supplier portal authentication.

- **RFC 7644 — SCIM 2.0 (System for Cross-domain Identity Management)**
  https://datatracker.ietf.org/doc/html/rfc7644
  Standard for automated user provisioning and lifecycle management across systems. Relevant for managing supplier portal user accounts, onboarding/offboarding supplier contacts, and syncing identity data across procurement platforms.

- **RFC 7519 — JSON Web Tokens (JWT)**
  https://datatracker.ietf.org/doc/html/rfc7519
  Compact token format used for secure information exchange between parties. Used in procurement API authentication flows and supplier portal session management.

- **RFC 7231 — HTTP/1.1 Semantics and Content**
  https://datatracker.ietf.org/doc/html/rfc7231
  Defines HTTP methods and status codes that form the foundation of RESTful API design for procurement platform integrations.

- **OpenID Connect Core 1.0**
  https://openid.net/specs/openid-connect-core-1_0.html
  Identity layer on top of OAuth 2.0 for SSO authentication. Enables federated login for supplier portals and cross-platform procurement access.

### Data Model & API Specifications

- **OpenAPI Specification 3.1 (OAS)**
  https://spec.openapis.org/oas/v3.1.0
  Vendor-neutral standard for describing RESTful APIs. Procurement platforms like Coupa and Veridion use OpenAPI-compatible REST APIs. Any new vendor discovery tool should publish its API using OAS for maximum interoperability.

- **JSON Schema (draft 2020-12)**
  https://json-schema.org/specification
  Standard for describing and validating JSON data structures. Used to define supplier profile schemas, RFI/RFP templates, and evaluation criteria data models.

- **GraphQL Specification**
  https://spec.graphql.org/
  Query language for APIs enabling clients to request exactly the data they need. Relevant for building flexible supplier search and filtering APIs where query complexity varies widely.

- **OASIS Universal Business Language (UBL) 2.3**
  https://docs.oasis-open.org/ubl/UBL-2.3.html
  Open library of standard electronic business documents for procurement including purchase orders, invoices, RFQs, and supplier qualification documents. Freely available without licensing fees.

- **PEPPOL Business Interoperability Specifications (BIS)**
  https://docs.peppol.eu/
  Framework for cross-border electronic procurement built on UBL. Defines standardised message formats for procurement processes including ordering, invoicing, and catalogue management. Mandatory for public procurement in many EU countries.

- **UN/SPSC (United Nations Standard Products and Services Code)**
  https://www.unspsc.org/
  Global taxonomy for classifying goods and services in procurement databases. Essential for categorising supplier capabilities and structuring RFI templates by product/service category.

### Security & Authentication Standards

- **OAuth 2.0 with PKCE (RFC 7636)**
  https://datatracker.ietf.org/doc/html/rfc7636
  Proof Key for Code Exchange extension for OAuth 2.0, recommended for public clients and single-page applications. Relevant for supplier portal web applications.

- **OWASP Application Security Verification Standard (ASVS)**
  https://owasp.org/www-project-application-security-verification-standard/
  Framework for testing web application security controls. Applicable to vendor discovery platforms handling sensitive supplier data and financial information.

- **NIST SP 800-161r1 — Cybersecurity Supply Chain Risk Management**
  https://csrc.nist.gov/publications/detail/sp/800-161/rev-1/final
  NIST guidelines for identifying, assessing, and mitigating cybersecurity risks in supply chains. Directly relevant to the vendor vetting and risk assessment components of the platform.

- **SOC 2 Type II**
  https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2
  Security and availability audit standard commonly required for SaaS vendor approvals. The platform itself should target SOC 2 compliance, and should track SOC 2 status as a supplier qualification criterion.

- **GDPR (General Data Protection Regulation)**
  https://gdpr.eu/
  EU data protection regulation affecting how supplier personal data (contacts, diversity status, financial information) is collected, processed, and stored. Particularly relevant for platforms operating in or serving EU markets.

- **SAML 2.0 (Security Assertion Markup Language)**
  https://docs.oasis-open.org/security/saml/v2.0/
  XML-based authentication standard for enterprise SSO. Commonly required for enterprise procurement platform deployments alongside OpenID Connect.

### MCP Server Specifications

- **Model Context Protocol (MCP)**
  https://modelcontextprotocol.io/
  Open protocol for connecting AI models to external data sources and tools. Relevant for building AI agent integrations that can autonomously search supplier databases, enrich profiles from external sources, and execute multi-step sourcing workflows.

- **MCP Tool Use Pattern**
  https://modelcontextprotocol.io/docs/concepts/tools
  MCP tool specification enabling AI agents to invoke structured actions (e.g., search suppliers, generate RFIs, score responses). An MCP server exposing vendor discovery and vetting capabilities could enable AI-native procurement agents to orchestrate sourcing workflows.

## Similar Products — Developer Documentation & APIs

### Coupa (including Scoutbee)
- **Description:** Leading AI platform for total spend management, with supplier discovery (via Scoutbee), procurement, invoicing, and payments.
- **API Documentation:** https://compass.coupa.com/en-us/products/product-documentation/integration-technical-documentation/the-coupa-core-api
- **Developer Docs (new):** https://docs.coupa.com/en/developer-documentation
- **SDKs/Libraries:** REST API with JSON and XML support; no public SDKs
- **Developer Guide:** https://compass.coupa.com/en-us/products/product-documentation/integration-technical-documentation/the-coupa-core-api/get-started-with-the-api
- **Standards:** RESTful API, UTF-8 XML and JSON, OAuth 2.0
- **Authentication:** OAuth 2.0 or API key

### SAP Ariba
- **Description:** Enterprise procurement platform with supplier discovery (SAP Business Network Discovery), sourcing, contract management, and procure-to-pay.
- **API Documentation:** https://developer.ariba.com/
- **SDKs/Libraries:** 190+ APIs covering procurement, sourcing, supplier management, catalogs, and analytics
- **Developer Guide:** https://developer.ariba.com/ (SAP Ariba APIs Portal)
- **Standards:** REST/JSON, cXML for commerce transactions, OpenAPI
- **Authentication:** OAuth 2.0, API key, certificate-based

### Veridion
- **Description:** AI-curated business data platform providing supplier search and enrichment APIs across 80M+ companies and 200M+ products.
- **API Documentation:** https://docs.veridion.com/
- **SDKs/Libraries:** REST API; no public SDKs disclosed
- **Developer Guide:** https://docs.veridion.com/ (Resource Hub with use cases and implementation guides)
- **Standards:** REST/JSON, API key authentication
- **Authentication:** API key

### GEP SMART
- **Description:** Unified procurement platform covering source-to-pay with supplier master data management, sourcing, contracts, and AP automation.
- **API Documentation:** Not publicly available; built-in adapters for ERP integration
- **SDKs/Libraries:** No public SDKs; built-in connectors for SAP, Oracle, JDE
- **Developer Guide:** https://www.gep.com/software/gep-smart/procurement-technology (GEP SMART CONNECT)
- **Standards:** REST API, ERP adapter framework
- **Authentication:** Enterprise SSO (SAML, OpenID Connect)

### Gatekeeper
- **Description:** Unified contract and third-party risk management platform with vendor lifecycle management, contract repository, and compliance tracking.
- **API Documentation:** Not publicly available; API access on Enterprise plan
- **SDKs/Libraries:** No-code custom data layer; 220+ native integrations, 1,700+ via connectors
- **Developer Guide:** https://www.gatekeeperhq.com/gatekeeper-interconnect
- **Standards:** REST API (Enterprise plan), Salesforce AppExchange, AWS Marketplace
- **Authentication:** SSO, RBAC (Enterprise plan)

### Zapro.ai
- **Description:** AI-native vendor management platform covering discovery, onboarding, procurement, AP automation, and performance management.
- **API Documentation:** Not publicly available
- **SDKs/Libraries:** No public SDKs or APIs disclosed
- **Developer Guide:** Not publicly available
- **Standards:** Proprietary SaaS with ERP integrations
- **Authentication:** Not publicly documented

### AutoRFP.ai
- **Description:** AI-powered RFP/RFI response automation platform that learns from past responses and approved content libraries.
- **API Documentation:** Not publicly available
- **SDKs/Libraries:** 18+ integrations including Salesforce, Google Drive, SharePoint, Notion, Intercom
- **Developer Guide:** Not publicly available
- **Standards:** Proprietary SaaS with native integrations
- **Authentication:** Not publicly documented

### Inventive.ai
- **Description:** AI RFP software with content governance, multi-language support, and deep integrations with engineering tools (Jira, GitHub, Confluence).
- **API Documentation:** Not publicly available
- **SDKs/Libraries:** Native integrations with Salesforce, Slack, Google Drive, SharePoint, Notion, Confluence, Zendesk, Jira, GitHub
- **Developer Guide:** Not publicly available
- **Standards:** Built on Azure AI; proprietary SaaS
- **Authentication:** Enterprise SSO (via Azure AD)

### Nvelop
- **Description:** AI-powered RFX management platform for RFP, RFQ, and RFI creation, distribution, scoring, and vendor matching.
- **API Documentation:** Not publicly available
- **SDKs/Libraries:** No public SDKs or APIs disclosed
- **Developer Guide:** Not publicly available
- **Standards:** GDPR-compliant with EU data residency
- **Authentication:** Not publicly documented

### Supplier.io (including TealBook)
- **Description:** Supplier intelligence and diversity platform with 20M+ supplier database, data enrichment, TrustIQ scoring, and Market Analyzer.
- **API Documentation:** Not publicly available (support documentation references API as developing feature)
- **SDKs/Libraries:** TealBook provides integrations with SAP Ariba, Coupa SIM, Oracle
- **Developer Guide:** Not publicly available
- **Standards:** Push-based data enrichment; batch and real-time sync
- **Authentication:** Not publicly documented

## Notes

**API maturity gap:** The vendor discovery and vetting space has a notable API maturity gap. Of the 10 platforms analysed, only Coupa, SAP Ariba, and Veridion offer publicly documented APIs. Most AI-native startups (Zapro, Nvelop, AutoRFP, Find My Factory) operate as closed platforms without developer-facing APIs. This represents a significant opportunity for an open-source, API-first alternative.

**Data format fragmentation:** There is no industry-standard data format for supplier profiles or evaluation records. Each platform defines its own schema. UBL covers transactional documents (POs, invoices) but does not define supplier qualification or vetting data models. A new entrant could differentiate by defining and open-sourcing a supplier profile schema.

**PEPPOL adoption expanding:** PEPPOL is mandatory for public procurement in many EU countries and expanding to Australia, New Zealand, and Singapore. Any platform targeting government or cross-border procurement should support PEPPOL BIS for document exchange.

**MCP as an emerging integration pattern:** The Model Context Protocol is emerging as a standard for connecting AI agents to external tools. Building an MCP server for vendor discovery would enable AI-native procurement agents to directly search, evaluate, and engage suppliers through any MCP-compatible AI platform.

**Emerging standards to watch:**
- **ISO 37000:2021 (Governance of Organizations)** — increasingly referenced in supplier governance frameworks
- **EU Corporate Sustainability Due Diligence Directive (CS3D)** — will require supply chain ESG due diligence, driving demand for automated supplier vetting
- **Digital Product Passport (EU)** — may require standardised supplier and component traceability data

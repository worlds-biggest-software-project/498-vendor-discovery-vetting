# Vendor Discovery & Vetting

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source platform that automates supplier discovery, RFI generation, and evaluation scoring -- replacing fragmented, expensive procurement toolchains with a single, transparent workflow.

Vendor Discovery & Vetting is an end-to-end supplier sourcing platform for procurement teams, strategic sourcing managers, and compliance officers. It addresses a core pain point in B2B procurement: finding, qualifying, and comparing vendors today requires stitching together 3-5 proprietary tools, each priced at USD 15k+/year, none of which offer transparent AI reasoning or cross-platform data portability. This project delivers the full cycle -- discovery, vetting, RFI automation, scoring, and continuous monitoring -- in a single open, API-first system.

---

## Why Vendor Discovery & Vetting?

- **Fragmented tooling forces expensive multi-vendor stacks.** No single incumbent covers discovery, vetting, RFI automation, scoring, and monitoring. Buyers must integrate Scoutbee for discovery, AutoRFP for responses, Tealbook for enrichment, and Gatekeeper for lifecycle management -- each with separate contracts and data silos.
- **AI-native sourcing is locked behind enterprise pricing.** Platforms like Zapro.ai start at USD 15k/year, and AI agent capabilities are gated to the highest tiers. SMBs and mid-market teams are shut out of advanced supplier intelligence.
- **Incumbent AI is a black box.** Most platforms deliver supplier rankings without explainable scoring rationale. Procurement teams cannot audit why a supplier was recommended or rejected, creating compliance and trust gaps.
- **Services procurement is underserved.** The strongest AI-native tools (Alibaba Accio, Find My Factory) are optimised for physical goods and manufacturing. Consulting, SaaS, and staffing vendor discovery remains largely manual.
- **Vendor data is trapped in proprietary platforms.** No standard export/import format exists for supplier profiles and evaluation history. Switching tools means rebuilding supplier databases from scratch.

---

## Key Features

### AI-Powered Supplier Discovery

- Natural language sourcing briefs replace keyword-based search -- describe what you need and receive a structured shortlist
- Multi-criteria filtering by industry, location, certifications, company size, and diversity status
- Automated supplier profile enrichment from public data sources, company websites, and regulatory filings
- Multimodal search supporting text, images, documents, and URLs (backlog)

### RFI/RFP Automation

- AI generates structured RFI/RFP documents from plain-language sourcing descriptions with appropriate evaluation criteria
- Template-driven creation with AI-assisted question drafting tailored to category and compliance requirements
- AI-powered response analysis comparing multiple supplier submissions side-by-side
- Trust Score attribution with source citations for every AI-generated answer

### Supplier Evaluation & Scoring

- Transparent, explainable scoring against weighted criteria with ranked shortlists
- Side-by-side comparison highlighting strengths, weaknesses, and compliance gaps
- Supplier diversity and ESG scoring with automated certification verification against official registries
- Balanced scorecards and review dashboards for ongoing supplier performance

### Compliance & Risk Monitoring

- Baseline compliance tracking for ISO 9001, ISO 14001, SOC 2 Type II, and diversity certifications
- Continuous supplier risk monitoring covering financial health signals, news, and regulatory changes
- NLP-based contract clause extraction identifying key terms, SLAs, and risk clauses
- Full audit trail with timestamp and user attribution

### Collaboration & Integration

- Team collaboration with role-based access control and approval workflows
- API-first architecture enabling integration with SAP Ariba, Coupa, and common ERP systems
- Supplier self-service portal for profile management and RFI responses (backlog)
- Cross-platform data portability with standard export/import for supplier profiles and evaluation history

---

## AI-Native Advantage

AI transforms vendor discovery from weeks of manual research into minutes of autonomous work. Agentic sourcing workflows conduct multi-step research across supplier databases, company websites, and regulatory filings to build qualified longlists from plain-language briefs. NLP evaluates supplier RFI responses side-by-side, assigns capability scores, and generates shortlist recommendations with transparent rationale -- something no incumbent offers at the scoring layer. Continuous monitoring uses NLP to track news, financial filings, and regulatory databases, flagging emerging supplier risks (bankruptcy, sanctions, compliance violations) before they become problems.

---

## Tech Stack & Deployment

The platform targets self-hosted, cloud, and hybrid deployment modes with an API-first architecture designed for developer integration. Key integration standards include DUNS (D-U-N-S) for supplier identity verification, UN/SPSC for goods and services classification, and ISO/SOC compliance frameworks for qualification workflows. REST APIs support search, enrichment, and scoring operations, with batch processing available for large-scale supplier data imports. Connectors for SAP Ariba, Coupa, Oracle, and major ERP systems are planned for the v1.1 release.

---

## Market Context

AI-driven procurement and vendor management sits within the broader USD 36 trillion B2B commerce market, with the procurement software segment valued in the tens of billions and AI-native tools capturing an increasing share. Incumbent pricing ranges from USD 15k-50k/year for mid-enterprise AI-native platforms to USD 100k+ for bundled enterprise suites -- leaving significant room for an open-source alternative. Primary buyers are procurement managers replacing manual supplier research, strategic sourcing teams managing complex multi-supplier evaluations, compliance officers ensuring regulatory and ESG qualification, and category managers benchmarking existing suppliers against alternatives.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.

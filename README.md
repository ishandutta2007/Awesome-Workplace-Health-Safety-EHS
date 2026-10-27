# Awesome-Workplace-Health-Safety-EHS

# Top Workplace Health & Safety (EHS) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Incident Management, Compliance Tracking & Field Safety Operations*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Workplace Health & Safety (EHS)**. These tools enable organizations to record incidents, manage corrective actions (CAPA), conduct inspections, track training and permits, and maintain regulatory compliance—protecting workers and reducing operational risk.

**Examples** include Workday Health and Safety, Cority, Intelex, VelocityEHS, Enablon, SafetyCulture (iAuditor), Quentic, Origami Risk, EcoOnline, and Benchmark ESG (the category leaders).

**Open-source emphasis**: EHS remains a challenging domain for open-source adoption—the projects below are either early-stage, narrowly scoped, or carry non-commercial licensing restrictions. The strongest active project is **SafetyMP Autonomous-EHS-Management**, which provides a self-hosted incident-to-CAPA spine with TRIR calculation. Teams seeking full EHS suites should plan for commercial platforms or significant custom development.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Workday Health and Safety](https://www.workday.com/)**  
  EHS capabilities within Workday's enterprise management cloud, integrating safety incidents, compliance tracking, and workforce data for unified risk visibility.

- **[Cority](https://www.cority.com/)**  
  Enterprise EHS and quality management platform covering incident management, audits, training, occupational health, and environmental compliance.

- **[Intelex](https://www.intelex.com/)**  
  EHS management software with incident tracking, inspections, compliance obligations, and analytics for industrial and manufacturing organizations.

- **[VelocityEHS](https://www.velocityehs.com/)**  
  EHS and ESG platform with incident management, chemical safety (SDS management), ergonomics, and control of work modules.

- **[Enablon](https://www.enablon.com/)**  
  Wolters Kluwer's EHS and operational risk management platform covering safety, environmental, and sustainability workflows for large enterprises.

- **[SafetyCulture (iAuditor)](https://safetyculture.com/)**  
  Mobile-first inspection and checklist platform with incident reporting, training, and corrective action tracking; widely adopted for field safety operations.

- **[Quentic](https://www.quentic.com/)**  
  EHS and ESG software with incident management, risk assessment, training management, and compliance workflows for European enterprises.

- **[Origami Risk](https://www.origamirisk.com/)**  
  Risk management platform with EHS modules covering incident reporting, claims management, and safety analytics.

- **[EcoOnline](https://www.ecoonline.com/)**  
  EHS and chemical safety platform with incident management, risk assessments, and compliance tracking for Nordic and European markets.

- **[Benchmark ESG](https://www.benchmarkesg.com/)**  
  ESG and EHS platform covering safety incidents, environmental compliance, and sustainability reporting.

## Open-Source GitHub Projects

- **[Autonomous-EHS-Management (SafetyMP)](https://github.com/SafetyMP/Autonomous-EHS-Management)**  
  The most complete active open-source EHS console (Apache 2.0); self-hosted on PostgreSQL with a core spine of **incident → linked CAPA → verified closure**; computes TRIR using `(recordable count × 200,000) / hours worked` with safeguards against incomplete monthly hour grids; includes demo fixtures for environmental permits, incident RCA (5 Whys/Ishikawa), risk registers, and program automation samples; Docker-deployable with optional AI for wording suggestions (a human closes records); explicitly does not claim OSHA certification or act as an official filing tool .

- **[BeaconHS](https://github.com/braedonsaunders/beaconhs)**  
  Open-source HSE platform for industrial construction (Next.js/PostgreSQL/TypeScript); features a visual **form builder** for JSAs, lift plans, confined-space permits, and toolbox talks; incidents, inspections, training, equipment, and permits modules; compliance hub rolling up obligations by entity, person, and site; multi-tenant with row-level security; includes an insights/BI engine and report builder; AI-assisted form generation with per-tenant model configuration .

- **[Digital Work Permit System](https://github.com/gauravdev148/Digital_Work_Permit_System)**  
  Open-source Permit-to-Work (PTW) system modeled as a **formal finite state machine** (Python/Flask) enforcing ISO 45001-aligned safety logic; prevents process-skipping by requiring mandatory `SAFETY_CHECK` and `APPROVAL` states before a permit can reach `ACTIVE`; includes visual state tracking and auditability of every transition .

### Additional Strong Open-Source Options

- **LOTO Management System** — Full-stack Lock Out Tag Out application (React/Node.js/MongoDB) with role-based access, multi-language support (EN/AR), and Docker deployment; addresses a specific but critical EHS control .
- **OiRA (osha.oira)** — EU-OSHA's Online Interactive Risk Assessment tool (Python/Plone); provides sector-specific risk assessment questionnaires with report generation; not a full EHS management system but a structured risk assessment foundation .
- **rEHS** — R package (Apache licensed, v0.1.0) offering a set of tools for EHS management; early-stage and limited in scope .

**Frameworks for building custom systems**: Combine **Autonomous-EHS-Management** for the incident-to-CAPA spine with TRIR reporting, **BeaconHS** for form-driven field inspections and permits with multi-tenant compliance tracking, and **Digital Work Permit System** for state-machine-enforced high-risk work authorization in a self-hosted EHS stack; layer **OiRA** for structured risk assessments where EU regulatory alignment is required.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- EHS platforms handling incident, injury, and worker health data must comply with applicable regulations (OSHA in the US, EU-OSHA directives, local labor laws, GDPR for personal data); incident records may be subject to regulatory retention and reporting requirements.
- **Open-source EHS remains significantly underdeveloped** compared to commercial platforms—Autonomous-EHS-Management provides a strong self-hosted spine for incident and CAPA workflows, but does not claim OSHA certification or official filing capability ; BeaconHS is early-stage but architecturally ambitious ; full enterprise EHS with chemical management, occupational health, and multi-jurisdictional compliance typically requires commercial platforms.
- Verify license terms for commercial use; Autonomous-EHS-Management uses Apache 2.0 , BeaconHS is open-source (check repository), and Digital Work Permit System is an independent open-source project .

---

**Made for EHS managers, safety officers, industrial hygienists, and operations leaders.**  
Let's make workplace health and safety more open, incident-aware, and worker-protective.

# Awesome-Healthcare-Hipaa-Compliance-Automation

# Top Healthcare HIPAA Compliance Automation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on PHI Sanitization, Audit Logging & Compliance Evidence Automation*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Healthcare HIPAA Compliance Automation**. These tools enable healthcare organizations, health tech developers, and covered entities to sanitize electronic health records during analysis, automate audit trails, and maintain compliance evidence—without manual review of every code commit or data pipeline.

**Examples** include Accountable, Compliancy Group, MedStack, Vanta Healthcare, Drata HIPAA, Protenus, Datica, Gazelle Consulting, Intraprise Health, and HIPAAtrek (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, PHI detection in CI/CD, and open audit logging—ideal for healthcare developers, compliance officers, and organizations seeking transparent, vendor-independent HIPAA automation.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Accountable](https://www.accountablehq.com/)**  
  All-in-one HIPAA compliance platform for healthcare startups and digital health companies. Features automated risk assessments, policy generation, employee training, and evidence collection. **Free tier available** for small teams.

- **[Compliancy Group](https://compliancy-group.com/)**  
  HIPAA compliance software with guided implementation, audit-ready documentation, and compliance coaching. Features **The Guard** for ongoing compliance management.

- **[MedStack](https://medstack.co/)**  
  Compliance-as-code platform for healthcare applications. **Automates HIPAA and SOC 2 infrastructure controls** at the container and orchestration layer—developers focus on code while MedStack handles security configuration.

- **[Vanta Healthcare](https://www.vanta.com/)**  
  Trust management platform with **HIPAA-specific automation**. Features continuous control monitoring, automated evidence collection, and auditor-ready reports. Covers HIPAA alongside SOC 2, ISO 27001, and GDPR.

- **[Drata HIPAA](https://drata.com/)**  
  Compliance automation with **HIPAA framework support**. Features automated evidence collection, control monitoring, and risk assessment. **No per-seat pricing**—flat platform fee.

- **[Protenus](https://www.protenus.com/)**  
  Healthcare compliance analytics platform. Uses **AI to monitor EHR access** and detect privacy violations, drug diversion, and insider threats. Provides **audit trail analysis** at scale.

- **[Datica (now Aizon)](https://datica.com/)**  
  HIPAA-compliant cloud platform for healthcare. Provides **compliant infrastructure** with BAA, encrypted storage, and audit logging. Acquired by Aizon.

- **[Gazelle Consulting](https://gazelleconsultingllc.com/)**  
  HIPAA compliance consulting and automation. Features risk assessment, policy templates, and ongoing compliance support.

- **[Intraprise Health](https://intraprisehealth.com/)**  
  HIPAA risk management platform. Features **security risk assessments**, vendor management, and compliance tracking.

- **[HIPAAtrek](https://hipaatrek.com/)**  
  HIPAA compliance management platform. Features **risk assessment, policy management, and audit trails**. Provides **BAAs** and compliance documentation.

## Open-Source GitHub Projects

- **[CISO Assistant](https://github.com/intuitem/ciso-assistant-community)**  
  **The most comprehensive open-source GRC platform with HIPAA support** (open-source). **3,000+ GitHub stars, 1,130+ forks** . One-stop-shop for GRC covering **Risk, AppSec, Compliance/Audit Management, Privacy**. Supports **+100 frameworks worldwide** with auto-mapping: **HIPAA**, NIST CSF, ISO 27001, SOC 2, CIS, PCI DSS, NIS2, CMMC, GDPR, DORA, NIST AI RMF, and more . **The most mature open-source compliance automation platform available.**

- **[baadiff](https://github.com/cognis-digital/baadiff)**  
  **HIPAA Security Rule readiness scanner for code** (open-source). **The most focused open-source HIPAA code auditor available.** **140+ rules across 5 HIPAA categories** mapped to specific CFR sections: Access Control (§164.312(a)(1)), Session Timeout (§164.312(a)(2)(iii)), Authentication Strength (§164.312(d)), Audit Logging (§164.312(b)), Encryption at Rest (§164.312(a)(2)(iv)), Integrity Controls (§164.312(c)(1)), Transmission Security (§164.312(e)(1)) . Features **CI gate** (exits non-zero below threshold), **MCP-native** (`baadiff mcp` exposes `scan()` to Claude Desktop, Cursor), **passive & offline** (reads local files only, no network, air-gapped CI safe) . **Polyglot ports** in Python, JavaScript, Go, Rust, and POSIX shell .

- **[verification-layer (vlayer)](https://github.com/Francosimon53/verification-layer)**  
  **Open-source HIPAA compliance scanner with 140+ rules and 5 HIPAA categories** (open-source). Features **CLI + CI/CD + VS Code extension** with real-time scanning on file save . **AI-powered scanning** (optional, via Claude) reduces false positives by **50%+** with **PHI scrubbing** (HIPAA-safe, no PHI sent to API). **White-label branding** for agencies and resellers. **Compliance dashboard (Pro)** with historical scans, team management, and audit reports .

- **[phi-guard](https://pypi.org/project/phi-guard/)**  
  **HIPAA PHI scanner for CI/CD pipelines** (open-source) — "like gitleaks, but for healthcare data." **The most CI-native open-source PHI detection tool available.** Scans for **17 of 18 HIPAA PHI types** including SSN, MRN, email, phone, dates, account numbers, and IP addresses . **Dual-mode architecture**: **pre-commit hook (fast regex, under 3 seconds)** blocks PHI before it reaches the repository; **CI/CD pipeline (full NLP via Microsoft Presidio)** catches names and locations that regex misses . **SARIF output** integrates with GitHub Security tab . **Custom healthcare recognizers** for MRN and insurance IDs, with stricter SSN detection than Presidio default .

- **[Health-DeID](https://pypi.org/project/health-deid/)**  
  **Local research software for auditable, resumable de-identification of clinical text** (open-source). **The most complete open-source clinical de-identification pipeline available.** Features **multiple detection backends**: AWS Comprehend Medical, **Claude Sonnet 4.6 on Amazon Bedrock**, local rules, or combination . **Retains, redacts, generalizes, date-shifts, or replaces** each PHI category . **Consistent replacements** by entity, record, or occurrence . **Optional validation** with GPT-OSS Safeguard 120B and **human review UI** . **Resumable runs** recover interrupted work and retain completed requests . **SQLite run database** for full audit trail .

- **[FHIR-READA](https://pypi.org/project/fhir-reada/)**  
  **FHIR Research Extractor And De-identified Analyzer** (MIT). **The most accessible open-source FHIR de-identification tool.** Python CLI for extracting, de-identifying, and exporting patient data from **any FHIR-compliant server** . Features **patient filtering by age range and diagnosis**, automatic **patient ID de-identification**, and **CSV export** . `fhir-reada --url https://r4.smarthealthit.org --min-age 25 --max-age 40 --diagnosis diabetes --out output.csv` .

- **[regulog](https://cran.r-project.org/web/packages/regulog/)**  
  **Tamper-evident audit logging for regulated environments** (open-source, CRAN). **The most rigorous open-source audit logging tool for HIPAA and FDA environments.** Records every action, change, note, and decision into a **tamper-evident, hash-chained audit trail** stored as newline-delimited JSON . Every entry is **attributed to a named user, time-stamped in UTC, and linked to the previous entry via SHA-256** — any modification is detectable by `verify_log()` . Works for **regulated pharmaceutical environments (21 CFR Part 11, EU Annex 11)** , internal data pipelines, multi-user Shiny applications. **Electronic signatures** with `log_signature()` . **Export to CSV/JSON for submission** .

- **[Aegis](https://github.com/RastinAghighi/Aegis)**  
  **HIPAA compliance auditor for code, powered by IBM Bob** (open-source). **The most AI-agent-integrated open-source HIPAA auditor available.** Features **MCP server** exposing six tools: `list_rules`, `scan_file`, `scan_repo`, `get_rule`, `get_remediation_template`, `generate_evidence` . **7 HIPAA rules implemented** as Rule subclasses with verbatim CFR text hardcoded: AC-1 (Access Control), AC-2 (Session Timeout), AC-3 (Authentication Strength), AU-1 (Audit Logging), EN-1 (Encryption at Rest), IN-1 (Integrity Controls), TR-1 (Transmission Security) . **Deterministic per-file scanning** with cross-file PHI flow analysis via MCP . **Auditor custom mode** with formal compliance persona enforcing citation-heavy language .

- **[hipaa-audit](https://www.npmjs.com/package/hipaa-audit)**  
  **CLI tool for running HIPAA compliance audits on codebases** (MIT, HackPrinceton Fall 2025). **The most accessible open-source HIPAA code auditor for quick assessment.** Features **API key verification**, **codebase collection** from 15+ file types, **compliance score (0-100)** with color-coded status (Green ≥80, Yellow 60-79, Red <60), **findings by severity** (Critical, High, Medium, Low), and **remediation plan** with prioritized fixes .

- **[HippocratAI](https://github.com/sparkybug/hippocrat-ai)**  
  **AI-powered clinical compliance reviewer for healthcare developers** (open-source, MIT). **The most comprehensive open-source multi-agent compliance reviewer.** Multi-agent pipeline activating on PR: **Agent 1** (Clinical Intent Analyzer), **Agent 2** (Regulatory Compliance: HIPAA, FDA 21 CFR Part 11, FHIR R4, IEC 62304), **Agent 3** (PubMed Research Agent), **Agent 4** (Standards Conflict Detector), **Agent 5** (Report Generator) . **Human approval checkpoint** before report reaches developer . **Overall status**: APPROVED / REQUIRES_CHANGES / BLOCKED .

- **[PhantomTrace](https://github.com/vabhishek6/PhantomTrace)**  
  **High-speed Rust tool to detect & mask PCI/PII in logs, text & streams** (open-source). **The fastest open-source PHI detection tool available.** Built for compliance (PCI DSS, GDPR, HIPAA). Features **configurable regex and ML detection**, **tokenization**, and **audit-ready reports** .

- **[Lynis](https://github.com/CISOfy/lynis)**  
  **Security auditing tool for Linux, macOS, and UNIX-based systems** (open-source). **The most mature open-source system hardening auditor for HIPAA/ISO27001/PCI DSS.** Agentless, installation optional . Assists with **compliance testing and system hardening** — a foundational layer for HIPAA security controls.

- **[Parse-HIPAA](https://github.com/netreconlab/parse-hipaa)**  
  **HIPAA & GDPR compliant ready parse-server with postgres/mongo** (open-source). **The most complete open-source HIPAA-compliant backend stack.** Compatible with **ParseCareKit** for healthcare applications. Includes **parse-hipaa-dashboard** for administration .

- **[SocialBright](https://github.com/HeidiStJacques/Social-Bright)**  
  **HIPAA-compliant, multi-tenant case management platform for social service organizations** (open-source). Features **client tracking, care planning, eligibility review, secure document storage, task management, and admin oversight** — all in one system .

- **[JukaleManmath/Healthcare-Record-Manager](https://github.com/JukaleManmath/Healthcare-Record-Manager)**  
  **AWS-Native Healthcare Record Automation Platform** (open-source). Features **Flask, PostgreSQL, Docker, CloudFormation, RBAC, HIPAA compliance, and comprehensive audit logging** .

- **[QMTRY-Healthcare-Compliance-Monitoring](https://github.com/daniel-QMTRY/QMTRY-Healthcare-Compliance-Monitoring)**  
  **Audit-ready healthcare compliance pipeline** (open-source). Features **dbt + Great Expectations + Streamlit** with **one-click GitHub Action** producing downloadable **evidence bundle for CMS, HIPAA, and NCQA/HEDIS** .

- **[ignition](https://github.com/castle-bravo-project/ignition)**  
  **Enterprise-grade compliance management and project orchestration platform with AI-powered automation** (open-source). Supports **ISO 27001, SOC 2, HIPAA, FDA standards** with intelligent project creation, automated assessments, and seamless GitHub integration .

- **[MCP-HIPAA](https://github.com/Gautam-Galada/MCP-HIPAA)**  
  **HIPAA-compliant medical AI agent built with MCP framework** (open-source). Features **role-based access control** and **local LLM inference**. Demonstrates **PHI data masking for doctors vs. unrestricted admin access**, with integrated X-ray analysis using TorchXRayVision .

### Additional Strong Open-Source Options

- **[DeIDClinic](https://github.com/angelpaulml17/DeIDClinic)** — Transformer-based clinical text de-identification with BioBERT/ClinicalBERT and comprehensive risk assessment (IEEE 2025) .
- **[FHIR-DIET](https://github.com/topics/hipaa)** — FHIR de-identification and pseudonymization service with YAML configuration rules, Web interface, CLI, and Docker deployment. Handles **~400 requests per second** in Web mode .
- **[DataGovernanceWorkflow](https://github.com/amr-yasser226/DataGovernanceWorkflow)** — Comprehensive data governance pipeline covering **GDPR/CCPA/HIPAA compliance** with encryption and classification .
- **[xk6-edi](https://github.com/cristofer1051/xk6-edi)** — Generate synthetic **HIPAA X12 EDI transactions** for load testing (837P/837D, 835, 270/271, 276/277) .
- Community **n8n** workflows for PHI detection alerting and compliance evidence routing.

**Frameworks for building custom systems**: Combine **phi-guard** for CI/CD PHI scanning with **Health-DeID** for clinical text de-identification, **regulog** for tamper-evident audit logging, **CISO Assistant** for GRC framework mapping, and **PostgreSQL** for persistence—creating a fully self-hosted, enterprise-grade HIPAA compliance automation platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- HIPAA compliance systems handling Protected Health Information (PHI) must comply with **HIPAA Privacy and Security Rules (45 CFR Parts 160 and 164)** , **HITECH Act**, and applicable state laws. **Legal review and qualified compliance expertise remain essential**—tools support automation, not legal advice.
- **Open-source HIPAA compliance automation is maturing but incomplete.** CISO Assistant provides comprehensive GRC framework mapping with HIPAA support . phi-guard provides CI-native PHI detection . Health-DeID provides clinical text de-identification . regulog provides tamper-evident audit logging . **No single open-source tool provides the end-to-end HIPAA compliance automation of Accountable or Compliancy Group.** Integration work is required.
- **A passing score is not certification.** baadiff explicitly states: "A passing score is **not** a HIPAA compliance certification, a risk analysis under §164.308(a)(1)(ii)(A), or legal advice. It is a static, best-effort readiness signal—a developer aid to catch obvious gaps early" . **Compliance requires organizational controls, workforce training, BAAs, and periodic risk assessments that tools cannot replace.**
- **PHI detection is probabilistic, not perfect.** phi-guard detects 17 of 18 PHI types (Names excluded to avoid false positives) . NLP-based detection in full mode catches unstructured PHI that regex misses, but false negatives remain possible. **Defense in depth—multiple detection engines and human review—is essential.**
- **Audit logs must be tamper-evident.** regulog's SHA-256 hash chain provides cryptographic proof that no entry has been altered . This is critical for HIPAA §164.312(b) audit controls and §164.308(a)(1)(ii)(D) system activity review .
- **Encryption remains a shared weakness in open-source EMRs.** A comparative benchmarking study found that **none of the evaluated EMRs (OpenEMR, OpenMRS, GNU Health, OSCAR EMR, Bahmni) provide native application-level encryption** for data at rest or file attachments, and **none offer integrated cryptographic key management** . This is an architectural gap requiring external solutions.
- Self-hosted open-source solutions require proper security hardening, BAA execution where applicable, and ongoing maintenance. **PHI is among the most sensitive data categories**—access controls, encryption, and audit trails are non-negotiable.

---

**Made for healthcare developers, compliance officers, privacy engineers, and developers building transparent HIPAA compliance solutions.**  
Let's make Healthcare HIPAA Compliance Automation more open, data-driven, and audit-ready.

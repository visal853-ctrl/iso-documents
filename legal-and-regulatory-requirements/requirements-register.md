# Requirements Register — Consolidated Legal, Regulatory & Contractual Requirements

## Document Control
- **Document ID**: LRR-REG-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal - Confidential
- **Owner**: Chief Compliance Officer (CCO)

---

## 1. Introduction

This **Requirements Register** provides a consolidated view of all legal, statutory, regulatory, and contractual requirements applicable to EuroTrust Bank AG's information security management system (ISMS). The register supports **ISO/IEC 27002:2022 Control 5.31** (Legal, statutory, regulatory and contractual requirements) by cataloguing obligations, assigning ownership, and tracking compliance status.

Each requirement in this register is derived from:
- **EU-wide regulations** (GDPR, PSD2, DORA, NIS2, eIDAS, EBA Guidelines, ECB expectations, AMLD, MiFID II, ePrivacy)
- **Country-specific regulations** (Germany, France, Netherlands, Spain, Poland, Ireland)
- **Contractual obligations** (AWS, PCI DSS, SWIFT CSP, correspondent banking, outsourcing, customer contracts, NDAs, cyber insurance, interbank networks, software licenses)

---

## 2. Requirements Register

### 2.1 Register Structure

The register includes the following columns:
- **Req ID**: Unique requirement identifier
- **Category**: Legal, Regulatory, or Contractual
- **Requirement Name**: Short description of the requirement
- **Reference/Source**: Legal citation, regulation number, contract reference
- **Jurisdiction**: Geographic scope (EU-wide, specific country, or global)
- **Applicable Business Area**: Business function or system affected
- **Key Information Security Obligations**: Summary of IS-related obligations
- **Compliance Owner**: Department or role responsible for compliance
- **Review Frequency**: How often compliance is reviewed
- **Last Reviewed**: Date of last compliance review
- **Status**: Compliant, In Progress, or Non-Compliant

---

### 2.2 Consolidated Requirements Table

| Req ID | Category | Requirement Name | Reference/Source | Jurisdiction | Applicable Business Area | Key IS Obligations | Compliance Owner | Review Frequency | Last Reviewed | Status |
|--------|----------|------------------|------------------|--------------|--------------------------|-------------------|------------------|------------------|---------------|--------|
| **EU-01** | Regulatory | GDPR — Data Protection Principles | Regulation (EU) 2016/679, Art. 5 | EU-wide (All 6 countries) | All operations processing personal data | Implement confidentiality, integrity, availability controls; data minimization; retention limits | DPO | Quarterly | Jan 2026 | Compliant |
| **EU-02** | Regulatory | GDPR — Security of Processing | Regulation (EU) 2016/679, Art. 32 | EU-wide | All IT systems | Implement state-of-the-art security: encryption, pseudonymization, resilience, incident recovery, regular testing | CISO | Quarterly | Jan 2026 | Compliant |
| **EU-03** | Regulatory | GDPR — Data Protection by Design & Default | Regulation (EU) 2016/679, Art. 25 | EU-wide | IT development, product design | Integrate privacy controls in system design; minimize data processing by default | CISO, DPO | Semi-annually | Jan 2026 | Compliant |
| **EU-04** | Regulatory | GDPR — Data Breach Notification (Authority) | Regulation (EU) 2016/679, Art. 33 | EU-wide | Incident response | Notify DPA within 72 hours of becoming aware of personal data breach | DPO, CISO | Ongoing (incident-driven) | Jan 2026 | Compliant |
| **EU-05** | Regulatory | GDPR — Data Breach Notification (Data Subjects) | Regulation (EU) 2016/679, Art. 34 | EU-wide | Incident response, customer communications | Notify affected data subjects without undue delay if high risk to rights and freedoms | DPO, Customer Service | Ongoing (incident-driven) | Jan 2026 | Compliant |
| **EU-06** | Regulatory | GDPR — Data Protection Impact Assessment (DPIA) | Regulation (EU) 2016/679, Art. 35 | EU-wide | High-risk processing activities | Conduct DPIA for high-risk data processing; document risks and mitigation | DPO, Business Units | Per new project/system | Jan 2026 | Compliant |
| **EU-07** | Regulatory | GDPR — International Data Transfers | Regulation (EU) 2016/679, Art. 44-50 | EU-wide | Cloud services, third-party vendors | Implement safeguards for data transfers outside EEA: adequacy decisions, SCCs, BCRs | DPO, Legal | Annually | Jan 2026 | Compliant |
| **EU-08** | Regulatory | PSD2 — Strong Customer Authentication (SCA) | Directive (EU) 2015/2366, Art. 95; RTS 2018/389 | EU-wide | Digital banking, payments | Implement multi-factor authentication (2 of 3 factors: knowledge, possession, inherence); dynamic linking | Head of Payments, CISO | Semi-annually | Dec 2025 | Compliant |
| **EU-09** | Regulatory | PSD2 — Protection of Payment Credentials | Directive (EU) 2015/2366, Art. 96 | EU-wide | Authentication systems | Secure storage of credentials; prevent unauthorized use; fraud detection | Head of Payments, CISO | Semi-annually | Dec 2025 | Compliant |
| **EU-10** | Regulatory | PSD2 — Incident Reporting to Regulator | Directive (EU) 2015/2366, Art. 97 | EU-wide | Payment systems | Report major operational/security incidents to national competent authority | Compliance Officer | Ongoing (incident-driven) | Dec 2025 | Compliant |
| **EU-11** | Regulatory | PSD2 — Security Audits | Directive (EU) 2015/2366, Art. 98 | EU-wide | Payment systems | Independent security audits at least annually | CISO, Head of Payments | Annually | Sep 2025 | Compliant |
| **EU-12** | Regulatory | DORA — ICT Risk Management Framework | Regulation (EU) 2022/2554, Art. 6 | EU-wide | All IT systems | Establish comprehensive ICT risk management framework; documented policies and procedures | CISO | Quarterly | Feb 2026 | Compliant |
| **EU-13** | Regulatory | DORA — ICT Incident Management | Regulation (EU) 2022/2554, Art. 9-13 | EU-wide | All IT systems | Detect, log, classify, respond to ICT incidents; report major incidents to regulator | CISO | Ongoing (incident-driven) | Feb 2026 | Compliant |
| **EU-14** | Regulatory | DORA — ICT Testing (Penetration Testing) | Regulation (EU) 2022/2554, Art. 17 | EU-wide | Critical IT systems | Conduct annual penetration testing; threat-led penetration testing (TLPT) every 3 years | CISO | Annually (TLPT: every 3 years) | Jan 2026 | Compliant |
| **EU-15** | Regulatory | DORA — ICT Third-Party Risk Management | Regulation (EU) 2022/2554, Art. 19-26 | EU-wide | Outsourcing, cloud services | Maintain register of ICT third parties; contractual security clauses; audit rights; exit strategies | CISO, Procurement | Annually | Feb 2026 | Compliant |
| **EU-16** | Regulatory | DORA — Critical ICT Third-Party Provider Oversight | Regulation (EU) 2022/2554, Art. 28-29 | EU-wide | Cloud services (AWS) | Assess concentration risk; notify authorities of critical provider arrangements | CISO, CRO | Annually | Feb 2026 | Compliant |
| **EU-17** | Regulatory | NIS2 — Cybersecurity Risk Management | Directive (EU) 2022/2555, Art. 21 | EU-wide (transposed nationally) | All IT systems | Implement risk analysis, incident handling, business continuity, supply chain security, cryptography, MFA | CISO | Quarterly | Feb 2026 | In Progress |
| **EU-18** | Regulatory | NIS2 — Incident Reporting | Directive (EU) 2022/2555, Art. 23 | EU-wide (transposed nationally) | All IT systems | Report significant incidents: early warning (24h), detailed report (72h), final report (1 month) | CISO, Compliance | Ongoing (incident-driven) | Feb 2026 | In Progress |
| **EU-19** | Regulatory | NIS2 — Governance (Board Oversight) | Directive (EU) 2022/2555, Art. 20 | EU-wide (transposed nationally) | Corporate governance | Management board approves and oversees cybersecurity risk management measures | Board, CISO | Annually | Feb 2026 | In Progress |
| **EU-20** | Regulatory | eIDAS — Qualified Electronic Signatures | Regulation (EU) No 910/2014, Art. 24 | EU-wide | Digital banking, contracts | Use qualified electronic signatures for legally binding documents; integration with QTSPs | Head of Digital Banking | Annually | Dec 2025 | Compliant |
| **EU-21** | Regulatory | eIDAS — Trust Service Security | Regulation (EU) No 910/2014, Art. 19 | EU-wide | PKI, digital signatures | Implement security measures for trust services; notify breaches to supervisory bodies | IT Security | Annually | Dec 2025 | Compliant |
| **EU-22** | Regulatory | EBA ICT Guidelines — ICT Governance | EBA/GL/2019/04, Section 4.1 | EU-wide | IT governance | Management body approves ICT strategy and risk appetite; clear roles and responsibilities | CISO, CIO | Annually | Jun 2025 | Compliant |
| **EU-23** | Regulatory | EBA ICT Guidelines — ICT Security | EBA/GL/2019/04, Section 5 | EU-wide | All IT systems | Information security policies (CIA); cryptography; network security; IAM; monitoring; physical security | CISO | Annually | Jun 2025 | Compliant |
| **EU-24** | Regulatory | EBA ICT Guidelines — ICT Third-Party Risk | EBA/GL/2019/04, Section 6 | EU-wide | Outsourcing | Due diligence on ICT third parties; contractual security clauses; ongoing monitoring | CISO, Procurement | Annually | Jun 2025 | Compliant |
| **EU-25** | Regulatory | EBA ICT Guidelines — ICT Business Continuity | EBA/GL/2019/04, Section 7 | EU-wide | All IT systems | BCP/DR plans; regular testing (at least annually); RTO/RPO definitions | CISO, CIO | Annually | Jun 2025 | Compliant |
| **EU-26** | Regulatory | ECB Cyber Resilience — Threat Intelligence | ECB Cyber Resilience Expectations | EU-wide (SSM banks) | Security operations | Establish threat intelligence capability; participate in information-sharing (FS-ISAC) | CISO | Ongoing | Q4 2025 | Compliant |
| **EU-27** | Regulatory | ECB Cyber Resilience — Penetration Testing & TLPT | ECB Cyber Resilience Expectations | EU-wide (SSM banks) | Critical IT systems | Regular penetration testing; TLPT framework participation | CISO | Annually (pen test); TLPT: Q3 2026 | Q4 2025 | Compliant |
| **EU-28** | Regulatory | AMLD 5 — Internal AML Controls & Data Protection | Directive (EU) 2018/843, Art. 32 | EU-wide | AML transaction monitoring | Risk management systems for AML; data protection when processing for AML purposes; 5-year record retention | CCO/MLRO | Semi-annually | Oct 2025 | Compliant |
| **EU-29** | Regulatory | MiFID II — Organizational Requirements (IT Security) | Directive 2014/65/EU, Art. 16(6) | EU-wide (wealth management) | Investment services, trading systems | Maintain systems to safeguard security, integrity, confidentiality; business continuity | Head of Wealth Mgmt, CISO | Annually | Sep 2025 | Compliant |
| **EU-30** | Regulatory | MiFID II — Record-Keeping | Directive 2014/65/EU, Art. 16(5) | EU-wide (wealth management) | Investment services | Retain records of services and transactions (minimum 5 years); accessible to authorities | Head of Wealth Mgmt, Compliance | Annually | Sep 2025 | Compliant |
| **EU-31** | Regulatory | ePrivacy — Confidentiality of Communications | Directive 2002/58/EC, Art. 5 | EU-wide | Email, messaging | Prohibition of interception/surveillance without consent; email encryption; secure messaging | CISO, IT | Annually | Nov 2025 | Compliant |
| **EU-32** | Regulatory | ePrivacy — Cookie Consent | Directive 2002/58/EC, Art. 5(3) | EU-wide | Website, online banking | Obtain consent for cookies (except strictly necessary); implement cookie consent management | DPO, Marketing | Annually | Nov 2025 | Compliant |
| **EU-33** | Regulatory | ePrivacy — Unsolicited Marketing | Directive 2002/58/EC, Art. 13 | EU-wide | Marketing | Prior consent for electronic marketing (email, SMS); opt-out mechanism | Marketing, DPO | Annually | Nov 2025 | Compliant |
| **DE-01** | Legal | BDSG — Employee Data Protection | BDSG Section 26 | Germany | HR systems | Specific rules for processing employee personal data; limitations on employee monitoring | DPO, HR | Annually | Jan 2026 | Compliant |
| **DE-02** | Regulatory | KWG Section 25a — IT Systems Security | KWG Section 25a | Germany | All IT systems (Germany HQ) | Adequate, comprehensible, secure IT systems; proper business organization; risk management | CRO, CISO | Ongoing | Q4 2025 | Compliant |
| **DE-03** | Regulatory | KWG Section 25b — Outsourcing Notification | KWG Section 25b | Germany | Cloud, IT outsourcing | Notification to BaFin for material outsourcing; written contracts; audit rights | CRO, Procurement | Per outsourcing arrangement | Q4 2025 | Compliant |
| **DE-04** | Regulatory | BAIT — Information Security Management System (ISMS) | BAIT Section 3 | Germany | All IT systems | Implement ISMS based on ISO 27001; information security policy approved by board; risk assessments | CISO | Semi-annually | Dec 2025 | Compliant |
| **DE-05** | Regulatory | BAIT — User Access Management | BAIT Section 4 | Germany | All IT systems | IAM process; least privilege; segregation of duties; quarterly access reviews | CISO, IT | Quarterly | Jan 2026 | Compliant |
| **DE-06** | Regulatory | BAIT — Data Backup & Disaster Recovery | BAIT Section 8 | Germany | Critical IT systems | Daily backups; off-site storage; documented DR plans; annual DR testing | CISO, CIO | Annually | Dec 2025 | Compliant |
| **DE-07** | Regulatory | IT-SiG 2.0 — Critical Infrastructure Security | IT-SiG 2.0, Section 8a BSIG | Germany | Critical infrastructure systems | State-of-the-art technical and organizational measures; report incidents to BSI | CISO | Annually | Q4 2025 | Compliant |
| **DE-08** | Regulatory | IT-SiG 2.0 — Detection Systems for Attacks | IT-SiG 2.0, Section 8b BSIG | Germany | All IT systems | Implement systems to detect attacks (SIEM, IDS/IPS); report detected attacks to BSI | CISO | Ongoing | Q4 2025 | Compliant |
| **FR-01** | Legal | Loi Informatique et Libertés — DPO Registration | Law No. 78-17 | France | Data protection | Appoint DPO; register with CNIL; biometric data governance | DPO | Annually | Jan 2026 | Compliant |
| **FR-02** | Regulatory | ACPR Guidelines — IT Governance & BCP | ACPR Guidelines | France | IT operations (France branch) | IT strategy aligned with business; BCP/DR plans; annual testing | Country Manager (FR), CISO | Annually | Q4 2024 | Compliant |
| **FR-03** | Regulatory | LPM — Critical Infrastructure (if OIV) | Military Programming Law | France | Critical systems (if designated OIV) | Security measures for critical systems; ANSSI oversight; incident reporting (if OIV designated) | CISO, Country Manager (FR) | Monitoring | Q4 2025 | Monitoring (not OIV) |
| **NL-01** | Legal | UAVG — Employee Data Processing | UAVG | Netherlands | HR systems (Netherlands) | Specific rules for employee monitoring; HR systems security | DPO, Country Manager (NL) | Annually | Jan 2026 | Compliant |
| **NL-02** | Regulatory | DNB Good Practices — Governance & Strategy | DNB Guidelines | Netherlands | IT operations (Netherlands, incl. Amsterdam DC) | Board oversight of IT/cybersecurity; IT strategy; three lines of defense | Country Manager (NL), CISO | Annually | Q4 2025 | Compliant |
| **NL-03** | Regulatory | DNB Good Practices — Operational Resilience (DR) | DNB Guidelines | Netherlands | Amsterdam data centre | BCP/DR; Amsterdam DC failover readiness; DR testing (Frankfurt ↔ Amsterdam) | Country Manager (NL), CISO | Annually | Q4 2025 | Compliant |
| **NL-04** | Regulatory | DNB Good Practices — Third-Party Risk | DNB Guidelines | Netherlands | Cloud, IT vendors | Due diligence on critical IT suppliers; concentration risk (AWS); exit planning | Country Manager (NL), CISO | Annually | Q4 2025 | Compliant |
| **ES-01** | Legal | LOPDGDD — Digital Rights & Employee Monitoring | Organic Law 3/2018 | Spain | HR systems, workplace monitoring | Digital disconnection rights; limitations on employee surveillance; AEPD registration | DPO, Country Manager (ES) | Annually | Jan 2026 | Compliant |
| **ES-02** | Regulatory | Banco de España Circulars — IT Governance & BCP | Circular 2/2016 | Spain | IT operations (Spain branch) | IT governance; BCP for Spanish branches; outsourcing notifications to Banco de España | Country Manager (ES), CISO | Annually | Q4 2025 | Compliant |
| **PL-01** | Legal | Polish Data Protection Act — DPO Registration | Act of 10 May 2018 | Poland | Data protection | Appoint DPO; register with UODO; security measures aligned with GDPR | DPO, Country Manager (PL) | Annually | Jan 2026 | Compliant |
| **PL-02** | Regulatory | National Cybersecurity System Act — Cybersecurity Risk Management | Act of 5 July 2018 | Poland | All IT systems (Poland) | Risk management systems; incident handling; business continuity; access control; cryptography; logging | CISO, Country Manager (PL) | Annually | Q4 2025 | Compliant |
| **PL-03** | Regulatory | National Cybersecurity System Act — Incident Reporting | Act of 5 July 2018 | Poland | All IT systems (Poland) | Report significant incidents to CSIRT NASK and KNF: initial (immediate), detailed (72h), final (1 month) | CISO, Country Manager (PL) | Ongoing (incident-driven) | Q4 2025 | Compliant |
| **PL-04** | Regulatory | National Cybersecurity System Act — Cybersecurity Audits | Act of 5 July 2018 | Poland | All IT systems (Poland) | Periodic cybersecurity audits (every 2 years) by certified auditors | CISO, Country Manager (PL) | Every 2 years | 2024 (next: 2026) | Compliant |
| **PL-05** | Regulatory | KNF Recommendations — IT Risk Management | KNF Recommendation D | Poland | IT operations (Poland) | IT risk management integrated into overall risk management; IT risk appetite; security policies | Country Manager (PL), CISO | Annually | Q4 2024 | Compliant |
| **IE-01** | Legal | Data Protection Act 2018 — DPO & Security Measures | Act No. 7 of 2018 | Ireland | Data protection | DPO appointment and independence; security measures based on risk; DPC registration | DPO, Country Manager (IE) | Annually | Jan 2026 | Compliant |
| **IE-02** | Regulatory | CBI Cross Industry Guidance — IT Governance | CBI Guidance (2016/2023) | Ireland | IT operations (Ireland) | Board oversight of IT/cybersecurity; IT strategy; risk assessments; ISO 27001 alignment | Country Manager (IE), CISO | Annually | Q4 2025 | Compliant |
| **IE-03** | Regulatory | CBI Cross Industry Guidance — Operational Resilience | CBI Guidance | Ireland | IT operations (Ireland) | BCP/DR capabilities; regular testing; cyber incident scenarios; RTO/RPO | Country Manager (IE), CISO | Annually | Q4 2025 | Compliant |
| **IE-04** | Regulatory | CBI Cross Industry Guidance — Third-Party Risk | CBI Guidance | Ireland | Cloud, IT vendors | Due diligence; contractual security clauses; ongoing monitoring; concentration risk | Country Manager (IE), CISO | Annually | Q4 2025 | Compliant |
| **CON-01** | Contractual | AWS — Data Processing Agreement & SCCs | AWS Customer Agreement, DPA, SCCs | Global (AWS EU regions) | Cloud services (AWS) | Data residency (EU regions); sub-processor approval; encryption (at rest & in transit); IAM; logging | CIO, CISO | Annually | Dec 2025 | Compliant |
| **CON-02** | Contractual | AWS — Security Incident Notification | AWS Customer Agreement | Global (AWS EU regions) | Cloud services (AWS) | AWS must notify EuroTrust of security incidents affecting customer data without undue delay | CIO, CISO | Ongoing (incident-driven) | Dec 2025 | Compliant |
| **CON-03** | Contractual | AWS — Right to Audit (Third-Party Reports) | AWS Customer Agreement | Global (AWS EU regions) | Cloud services (AWS) | Review AWS compliance reports (SOC 2, ISO 27001) annually as evidence of security controls | CISO | Annually | Dec 2025 | Compliant |
| **CON-04** | Contractual | PCI DSS — Cardholder Data Environment (CDE) Security | PCI DSS v4.0 | Global | Payment card systems | Implement all 12 PCI DSS requirements (300+ sub-requirements); network segmentation; encryption; access control; logging; testing | Head of Payments, CISO | Quarterly (scans), Annually (QSA) | Sep 2025 | Compliant |
| **CON-05** | Contractual | PCI DSS — Quarterly Vulnerability Scans | PCI DSS Requirement 11 | Global | Payment card systems | Quarterly external vulnerability scans by ASV; remediate vulnerabilities rated 4.0+ (CVSS) | CISO, IT Security | Quarterly | Jan 2026 | Compliant |
| **CON-06** | Contractual | PCI DSS — Annual Assessment (QSA) | PCI DSS Compliance Validation | Global | Payment card systems | Annual on-site assessment by QSA; Report on Compliance (ROC); Attestation of Compliance (AOC) | Head of Payments, Compliance | Annually | Sep 2025 | Compliant |
| **CON-07** | Contractual | SWIFT CSP — Mandatory Security Controls | SWIFT CSP 2025, CSCF | Global | SWIFT systems | Implement 21 mandatory SWIFT CSP controls (secure environment, access mgmt, patching, monitoring, IR) | Head of Treasury, CISO | Annually | Dec 2025 | Compliant |
| **CON-08** | Contractual | SWIFT CSP — Annual Attestation | SWIFT CSP | Global | SWIFT systems | Self-attest compliance with SWIFT CSP by year-end; independent assessment recommended | Head of Treasury, CISO | Annually | Dec 2025 | Compliant |
| **CON-09** | Contractual | SWIFT CSP — Incident Reporting to SWIFT | SWIFT CSP | Global | SWIFT systems | Report cyber incidents affecting SWIFT infrastructure/messaging to SWIFT CSIR portal ASAP | Head of Treasury, CISO | Ongoing (incident-driven) | Dec 2025 | Compliant |
| **CON-10** | Contractual | Correspondent Banking — Security Questionnaires | Various correspondent agreements | Global | Treasury, payments | Respond to correspondent cybersecurity questionnaires; share SWIFT CSP attestation | Head of Treasury, Compliance | Annually (or upon request) | Q4 2025 | Compliant |
| **CON-11** | Contractual | Correspondent Banking — Incident Notification | Various correspondent agreements | Global | Treasury, payments | Notify correspondents of incidents affecting payment processing or correspondent relationship | Head of Treasury, Compliance | Ongoing (incident-driven) | Q4 2025 | Compliant |
| **CON-12** | Contractual | Outsourcing (EBA) — Written Contracts with Security Clauses | EBA Outsourcing Guidelines, Vendor contracts | EU-wide | All outsourcing arrangements | Security and confidentiality clauses; audit rights; subcontracting approval; incident notification; exit rights | Procurement, CISO | Per contract (ongoing monitoring) | Q1 2026 | Compliant |
| **CON-13** | Contractual | Outsourcing (EBA) — Due Diligence & Risk Assessment | EBA Outsourcing Guidelines | EU-wide | All outsourcing arrangements | Conduct vendor risk assessment before outsourcing; review security certifications (SOC 2, ISO 27001) | CISO, Procurement | Per new vendor | Q1 2026 | Compliant |
| **CON-14** | Contractual | Outsourcing (EBA) — Notification to Regulators | EBA Outsourcing Guidelines | EU-wide | Material outsourcing | Notify national competent authorities (BaFin, ACPR, DNB, etc.) of material outsourcing before commencement | Compliance Officer | Per material outsourcing | Q1 2026 | Compliant |
| **CON-15** | Contractual | Customer Contracts — GDPR Privacy Notice | Customer terms & conditions, GDPR | EU-wide | Customer-facing systems | Provide privacy notice at account opening; describe data processing, security measures, data subject rights | DPO, Legal | Annually (or upon material change) | Nov 2025 | Compliant |
| **CON-16** | Contractual | Customer Contracts — Data Breach Notification to Customers | Customer terms & conditions, GDPR Art. 34 | EU-wide | Customer-facing systems | Notify customers of personal data breaches if high risk to rights/freedoms without undue delay | DPO, Customer Service | Ongoing (incident-driven) | Nov 2025 | Compliant |
| **CON-17** | Contractual | Customer Contracts — Data Subject Rights (DSARs) | Customer terms & conditions, GDPR | EU-wide | Customer-facing systems | Facilitate exercise of data subject rights (access, rectification, erasure, portability); respond within 1 month | DPO, IT | Ongoing (upon request) | Nov 2025 | Compliant |
| **CON-18** | Contractual | NDAs — Confidentiality & Security Measures | Various NDAs with third parties | Global | Third-party relationships | Protect confidential information; implement reasonable security measures; restrict disclosure | Legal, CISO | Per NDA (ongoing) | Ongoing | Compliant |
| **CON-19** | Contractual | NDAs — Breach Notification | Various NDAs | Global | Third-party relationships | Notify EuroTrust immediately upon discovery of unauthorized disclosure or breach of confidential information | Legal, CISO | Ongoing (incident-driven) | Ongoing | Compliant |
| **CON-20** | Contractual | Cyber Insurance — Maintain Security Controls | Cyber insurance policy | Global | All IT systems | Maintain security controls represented in insurance application (MFA, encryption, patching, IR, backups) | CRO, CISO | Annually (renewal) | Nov 2025 | Compliant |
| **CON-21** | Contractual | Cyber Insurance — Incident Notification to Insurer | Cyber insurance policy | Global | Incident response | Notify insurer of cyber incidents that may give rise to claim within 72 hours | CRO, CISO | Ongoing (incident-driven) | Nov 2025 | Compliant |
| **CON-22** | Contractual | Interbank Networks — Operational Security (Availability) | SEPA, TARGET2, EBA Clearing rulebooks | EU-wide (Eurozone) | Payment systems | Ensure availability of payment systems during operating hours (99.9% uptime); BCP/DR | Head of Treasury, IT | Ongoing | Q1 2026 | Compliant |
| **CON-23** | Contractual | Interbank Networks — Incident Reporting | SEPA, TARGET2, EBA Clearing rulebooks | EU-wide (Eurozone) | Payment systems | Notify network operators (TARGET2, EBA Clearing) of incidents affecting payment processing | Head of Treasury, Compliance | Ongoing (incident-driven) | Q1 2026 | Compliant |
| **CON-24** | Contractual | Software Licenses — License Compliance & SAM | Microsoft, CrowdStrike, Splunk, other vendors | Global | All IT systems | Use software in accordance with license terms; maintain software asset management (SAM) program | CIO, IT Asset Mgmt | Annually | Q4 2025 | Compliant |
| **CON-25** | Contractual | Software Licenses — Security Configurations & Patching | Vendor licensing agreements | Global | All IT systems | Implement vendor-recommended security configurations; apply security patches in timely manner | CISO, IT Operations | Ongoing (patch mgmt) | Ongoing | Compliant |

---

## 3. Summary Statistics

### 3.1 Requirements by Category
- **EU-wide Regulatory**: 33 requirements (EU-01 through EU-33)
- **Country-Specific Legal/Regulatory**: 24 requirements (DE-01 through IE-04)
- **Contractual**: 25 requirements (CON-01 through CON-25)
- **Total Requirements**: **82 requirements**

### 3.2 Requirements by Jurisdiction
- **EU-wide**: 58 requirements
- **Germany**: 8 requirements
- **France**: 3 requirements
- **Netherlands**: 4 requirements
- **Spain**: 2 requirements
- **Poland**: 5 requirements
- **Ireland**: 4 requirements
- **Global (contractual)**: 25 requirements

### 3.3 Requirements by Compliance Status
- **Compliant**: 79 requirements (96%)
- **In Progress**: 3 requirements (4%) — NIS2 implementation (EU-17, EU-18, EU-19) [transposition ongoing in member states]
- **Non-Compliant**: 0 requirements

### 3.4 Requirements by Owner
- **CISO**: Primary or shared ownership of 58 requirements
- **DPO**: Primary or shared ownership of 19 requirements
- **Compliance Officer**: Primary or shared ownership of 15 requirements
- **CRO**: Primary or shared ownership of 8 requirements
- **Head of Payments**: Primary ownership of 6 requirements
- **Head of Treasury**: Primary ownership of 7 requirements
- **CIO**: Primary or shared ownership of 9 requirements
- **Legal**: Primary ownership of 5 requirements
- **Business Unit Heads** (Wealth Mgmt, Digital Banking, Marketing): 8 requirements
- **Country Managers**: 12 requirements

---

## 4. Compliance Monitoring & Review

### 4.1 Review Frequencies
- **Ongoing (Incident-Driven)**: Incident reporting obligations (EU-04, EU-05, EU-10, EU-13, etc.)
- **Quarterly**: High-priority regulatory obligations (GDPR, DORA, NIS2, BAIT access reviews, PCI DSS scans)
- **Semi-Annually**: PSD2, AMLD, BAIT reviews
- **Annually**: Country-specific regulations, contractual obligations, third-party reviews, certifications
- **Multi-Year**: TLPT (every 3 years), Polish cybersecurity audits (every 2 years)

### 4.2 Monitoring Mechanisms
1. **Regulatory Horizon Scanning**: Legal and Compliance teams monitor legislative changes (monthly updates)
2. **Compliance Calendar**: Automated reminders for review deadlines (integrated in GRC tool)
3. **Incident-Driven Notifications**: Incident response process includes automated regulatory notification checks
4. **Third-Party Monitoring**: Vendor management system tracks vendor compliance status (annual reviews)
5. **Internal Audits**: Internal Audit conducts periodic audits of compliance with key requirements
6. **Management Reporting**: Quarterly compliance reports to Executive Committee and Board Risk Committee

### 4.3 Escalation Process
- **Non-Compliance Identified** → Immediate escalation to requirement owner and CCO → Root cause analysis and remediation plan → Executive Committee notification (if material) → Regulator notification (if required by law/contract)
- **Deadline at Risk** → Early warning to requirement owner (30 days before deadline) → Escalation to CCO (15 days before deadline) → Executive Committee notification (if unresolved)

---

## 5. Cross-Cutting Themes & Interdependencies

### 5.1 Incident Reporting
**Overlapping obligations** require coordination:
- **GDPR**: 72 hours to DPA (if personal data breach)
- **PSD2**: Report major operational/security incidents to national competent authority
- **DORA**: Report major ICT incidents to regulator
- **NIS2**: 24h early warning, 72h detailed report, 1 month final report
- **National Laws**: Germany (IT-SiG 2.0 to BSI), Poland (to CSIRT NASK and KNF), etc.
- **Contractual**: AWS, SWIFT, correspondents, insurer (within 72h)

**Coordination Mechanism**: **Centralized incident response process** with **regulatory notification matrix** mapping incident types to notification obligations.

### 5.2 Third-Party Risk Management
**Multiple requirements mandate vendor risk management**:
- DORA, EBA Outsourcing Guidelines, NIS2, DNB Guidelines, CBI Guidance, country-specific regulations
- **Contractual**: AWS DPA/SCCs, outsourcing agreements, NDAs

**Coordination Mechanism**: **Enterprise vendor risk management program** with **centralized vendor register** and **standardized due diligence process**.

### 5.3 Encryption & Cryptography
**Requirements**: GDPR (Art. 32), DORA, EBA Guidelines, NIS2, BAIT, PCI DSS, AWS DPA, SWIFT CSP, ePrivacy
- **Standards**: AES-256 (data at rest), TLS 1.3 (data in transit), strong key management

### 5.4 Penetration Testing
**Requirements**: DORA (annual + TLPT every 3 years), PSD2 (annual), PCI DSS (annual), ECB expectations
- **Coordination**: **Unified penetration testing program** with annual external tests and TLPT every 3 years.

### 5.5 Business Continuity & Disaster Recovery
**Requirements**: DORA, EBA Guidelines, BAIT, MiFID II, NIS2, DNB Guidelines, CBI Guidance, AWS SLAs, SWIFT CSP, interbank networks
- **Coordination**: **Enterprise BCP/DR program** with annual testing, RTO/RPO definitions, failover between Frankfurt and Amsterdam data centres.

---

## 6. Gap Analysis & Continuous Improvement

### 6.1 Current Gaps
- **NIS2 Transposition** (EU-17, EU-18, EU-19): National transpositions in progress (deadline: October 2024, passed; implementations ongoing in some countries). **Action**: Monitor national implementations; update policies and procedures as national laws are finalized.

### 6.2 Continuous Improvement Initiatives
1. **ISO 27001:2022 Certification** (Target: Q4 2026): Formalize ISMS aligned with all regulatory and contractual requirements
2. **Zero Trust Architecture**: Multi-year program to enhance security (network segmentation, micro-segmentation, identity-centric security)
3. **Enhanced Threat Detection**: SOC maturity improvement (SOAR implementation, advanced threat hunting)
4. **Supply Chain Security**: Enhanced third-party risk management (continuous monitoring, security ratings)

---

## 7. Document Maintenance

### 7.1 Update Process
1. **Legislative/Regulatory Changes** → Legal/Compliance analysis → Impact assessment → Update requirements register → Communicate to owners → Update policies/procedures → Training (if needed)
2. **Contractual Changes** → Legal review → Update register → Communicate to owners
3. **Internal Changes** (e.g., new systems, new vendors) → Impact assessment → Update register → Document new obligations

### 7.2 Review Schedule
- **Frequency**: Quarterly (or upon material change)
- **Owner**: Chief Compliance Officer
- **Next Scheduled Review**: April 2026

### 7.3 Version Control
- Version history maintained in document header
- Changes tracked and approved by CCO

---

## 8. Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Compliance Team | Initial version with 82 requirements for ISO 27001 audit |

---

**END OF DOCUMENT**

# Compliance Approach — Legal, Regulatory & Contractual Requirements

## Document Control
- **Document ID**: LRR-CA-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal
- **Owner**: Chief Compliance Officer (CCO)

---

## 1. Introduction

This document describes **EuroTrust Bank AG's approach to meeting legal, statutory, regulatory, and contractual requirements** related to information security. It establishes the governance structure, roles and responsibilities, processes, and mechanisms for identifying, monitoring, and ensuring compliance with applicable requirements.

This document supports **ISO/IEC 27002:2022 Control 5.31** (Legal, statutory, regulatory and contractual requirements) and demonstrates the organization's systematic approach to managing compliance obligations.

---

## 2. Scope

This compliance approach applies to:
- **EU-wide regulations**: GDPR, PSD2, DORA, NIS2, eIDAS, EBA Guidelines, ECB supervisory expectations, AMLD, MiFID II, ePrivacy
- **Country-specific regulations**: National laws and regulations in Germany, France, Netherlands, Spain, Poland, and Ireland
- **Contractual obligations**: Agreements with cloud providers (AWS), payment networks (PCI DSS, SWIFT), correspondents, outsourcing vendors, customers, insurers, and other third parties
- **All EuroTrust Bank AG operations**: Headquarters (Frankfurt), branches (Paris, Amsterdam, Madrid, Warsaw, Dublin), and all employees, systems, and processes

---

## 3. Governance Structure for Legal & Regulatory Compliance

### 3.1 Three Lines of Defense Model

EuroTrust Bank AG adopts the **Three Lines of Defense** model for compliance governance:

#### 3.1.1 First Line of Defense: Business Units
- **Responsibility**: Own and manage compliance risks; implement controls
- **Activities**:
  - Execute day-to-day compliance with legal, regulatory, and contractual requirements
  - Implement policies, procedures, and controls mandated by requirements
  - Conduct self-assessments and monitoring
  - Escalate compliance issues to Compliance function (second line)
- **Examples**: Country Managers, Head of Payments, Head of Digital Banking, IT teams, Operations

#### 3.1.2 Second Line of Defense: Compliance, Risk, and Information Security Functions
- **Responsibility**: Oversee, monitor, and challenge the first line; provide guidance and support
- **Functions**:
  - **Compliance Function** (led by CCO): Interpret regulations, develop compliance programs, monitor adherence, report to regulators
  - **Risk Management Function** (led by CRO): IT risk assessments, operational risk management, third-party risk
  - **Information Security Function** (led by CISO): Implement technical and organizational security measures; cybersecurity risk management
  - **Data Protection Function** (led by DPO): GDPR and data protection compliance; privacy risk management
  - **Legal Function** (led by Chief Legal Officer): Interpret laws and contracts, provide legal advice, manage contractual compliance

- **Activities**:
  - Identify and interpret legal, regulatory, and contractual requirements
  - Develop policies, standards, and procedures
  - Conduct compliance monitoring, testing, and reviews
  - Provide training and awareness
  - Report to executive management and Board
  - Interface with regulators and external auditors

#### 3.1.3 Third Line of Defense: Internal Audit
- **Responsibility**: Provide independent assurance on effectiveness of compliance framework
- **Activities**:
  - Conduct periodic audits of compliance with legal, regulatory, and contractual requirements
  - Test effectiveness of controls
  - Report audit findings to Audit Committee
  - Follow up on remediation of audit issues

### 3.2 Organizational Chart (Compliance Governance)

```
Board of Directors
├── Audit Committee
│   └── Internal Audit (3rd Line)
└── Board Risk Committee
    └── Executive Committee
        ├── Chief Executive Officer (CEO)
        ├── Chief Compliance Officer (CCO) — 2nd Line
        │   ├── Compliance Team (15 staff)
        │   └── Country Compliance Officers (6 countries)
        ├── Chief Risk Officer (CRO) — 2nd Line
        │   ├── IT Risk Team
        │   └── Third-Party Risk Team
        ├── Chief Information Security Officer (CISO) — 2nd Line
        │   ├── Information Security Team (80 staff)
        │   └── Security Operations Centre (SOC)
        ├── Data Protection Officer (DPO) — 2nd Line
        │   └── Data Protection Team (40 staff)
        ├── Chief Legal Officer
        │   └── Legal Counsel Team (120 staff)
        └── Business Unit Heads (1st Line)
            ├── Country Managers (Germany, France, NL, Spain, Poland, Ireland)
            ├── Head of Payments & Digital Banking
            ├── Head of Treasury
            ├── Head of Wealth Management
            ├── Chief Information Officer (CIO) — IT Operations
            └── Other business units
```

---

## 4. Roles & Responsibilities

### 4.1 Board of Directors
- **Responsibilities**:
  - Approve corporate compliance strategy and risk appetite
  - Oversee management's implementation of compliance framework
  - Receive quarterly compliance reports from CCO and CISO
  - Approve key policies (e.g., Information Security Policy, Data Protection Policy)
  - Ensure adequate resources for compliance functions

### 4.2 Board Risk Committee
- **Responsibilities**:
  - Oversee enterprise risk management, including legal, regulatory, and compliance risks
  - Review and challenge management's compliance assessments and risk appetite
  - Approve major compliance programs (e.g., DORA implementation, NIS2 compliance)
  - Receive incident reports for significant compliance breaches

### 4.3 Audit Committee
- **Responsibilities**:
  - Oversee Internal Audit function
  - Review internal audit findings on compliance
  - Monitor remediation of compliance issues identified by Internal Audit or regulators

### 4.4 Chief Executive Officer (CEO)
- **Responsibilities**:
  - Ultimate accountability for compliance with legal, regulatory, and contractual requirements
  - Set tone at the top for compliance culture
  - Approve compliance strategy and allocate resources
  - Accountable to Board for compliance performance

### 4.5 Chief Compliance Officer (CCO)
- **Responsibilities**:
  - Lead the Compliance function (second line of defense)
  - Develop and maintain the **Compliance Framework**
  - Identify, interpret, and monitor legal and regulatory requirements
  - Develop and deliver compliance policies, procedures, and training
  - Coordinate with regulators (BaFin, ECB, national authorities)
  - Investigate and report compliance breaches
  - Quarterly compliance reporting to Executive Committee and Board Risk Committee
  - Chair the **Compliance Committee** (monthly meetings)
  - Escalate material compliance issues to CEO and Board

- **Direct Reports**:
  - Head of Regulatory Compliance (EU-wide regulations)
  - Head of Financial Crime Compliance (AML/CFT, sanctions)
  - Compliance Risk Manager
  - Country Compliance Officers (6 countries)

### 4.6 Chief Risk Officer (CRO)
- **Responsibilities**:
  - Lead Enterprise Risk Management (ERM) function
  - IT risk management and operational risk oversight
  - Third-party risk management (vendor risk assessments, outsourcing governance)
  - Business continuity management (BCP/DR)
  - Risk appetite framework and risk reporting
  - Interface with ECB and national banking supervisors on prudential and operational risk matters
  - Chair the **Enterprise Risk Committee** (monthly meetings)

- **Supporting Teams**:
  - IT Risk Team (IT risk assessments, alignment with DORA, EBA Guidelines)
  - Third-Party Risk Committee (vendor risk governance)
  - Business Continuity Team

### 4.7 Chief Information Security Officer (CISO)
- **Responsibilities**:
  - Lead the Information Security function (second line of defense for cybersecurity)
  - Develop, implement, and maintain the **Information Security Management System (ISMS)** (ISO 27001)
  - Cybersecurity risk management (aligned with DORA, NIS2, BAIT, EBA Guidelines)
  - Security architecture, security operations (SOC), incident response, vulnerability management, penetration testing
  - Interface with national cybersecurity authorities (BSI in Germany, ANSSI in France, CSIRT NASK in Poland, etc.)
  - Report security incidents to regulators (DORA, NIS2, IT-SiG 2.0, national cybersecurity laws)
  - Compliance with technical security requirements (PCI DSS, SWIFT CSP, AWS security, etc.)
  - Quarterly security reporting to Executive Committee and Board Risk Committee
  - Chair the **Information Security Council** (monthly meetings)

- **Direct Reports**:
  - Deputy CISO / Head of Security Operations (SOC)
  - Head of Security Architecture & Engineering
  - Head of Cyber Threat Intelligence
  - Head of Identity & Access Management (IAM)
  - Head of Security Governance, Risk & Compliance (InfoSec GRC)
  - Country Information Security Leads (6 countries)

### 4.8 Data Protection Officer (DPO)
- **Responsibilities**:
  - Lead the Data Protection function (GDPR compliance)
  - Interpret and advise on GDPR and national data protection laws
  - Monitor compliance with GDPR (Art. 5-10, Art. 32-34, etc.)
  - Conduct Data Protection Impact Assessments (DPIAs)
  - Handle data subject access requests (DSARs) and data subject rights
  - Report personal data breaches to data protection authorities (DPAs) and affected individuals
  - Interface with DPAs (BfDI in Germany, CNIL in France, AP in Netherlands, AEPD in Spain, UODO in Poland, DPC in Ireland, EDPB at EU level)
  - Maintain **Register of Processing Activities** (GDPR Art. 30)
  - Provide data protection training to employees
  - Chair the **Data Protection Forum** (bi-monthly meetings)
  - Report to Board on data protection compliance (via CCO)

- **Independence**: DPO reports directly to highest management level (CEO); independent from business units; cannot be instructed on how to perform DPO tasks

- **Direct Reports**:
  - Data Protection Advisors (embedded in business units)
  - Data Privacy Analysts
  - Country Data Protection Liaisons (6 countries)

### 4.9 Chief Legal Officer / Legal Counsel
- **Responsibilities**:
  - Provide legal advice on interpretation of laws, regulations, and contracts
  - Draft, review, and negotiate contracts (including security clauses in outsourcing agreements, DPAs, NDAs)
  - Monitor legislative and regulatory developments (legal horizon scanning)
  - Represent EuroTrust Bank AG in regulatory investigations and enforcement actions
  - Manage litigation related to compliance breaches
  - Coordinate with external legal counsel

- **Supporting Teams**:
  - Regulatory Affairs Team (monitoring regulatory changes)
  - Contracts Team (contract management and review)
  - Litigation & Investigations Team

### 4.10 Country Managers
- **Responsibilities** (for each of the 6 countries):
  - Ensure compliance with country-specific legal and regulatory requirements
  - Act as first line of defense for country-specific compliance
  - Liaise with national regulators and authorities (banking supervisors, DPAs, cybersecurity authorities)
  - Implement Group policies and adapt to local legal requirements where necessary
  - Escalate country-specific compliance issues to CCO and CISO

- **Support**: Country Compliance Officers (reporting to CCO), Country Information Security Leads (reporting to CISO)

### 4.11 Business Unit Heads (First Line)
- **Examples**: Head of Payments, Head of Treasury, Head of Digital Banking, Head of Wealth Management, CIO (IT Operations)
- **Responsibilities**:
  - Own and manage compliance risks within their business areas
  - Implement policies, procedures, and controls mandated by compliance requirements
  - Ensure employees are trained on relevant compliance obligations
  - Report compliance issues and incidents to Compliance, Risk, or CISO as appropriate
  - Participate in compliance assessments, audits, and reviews

### 4.12 Internal Audit (Third Line)
- **Responsibilities**:
  - Provide independent assurance on effectiveness of compliance framework
  - Conduct risk-based audits of compliance with legal, regulatory, and contractual requirements
  - Test design and operating effectiveness of compliance controls
  - Report audit findings to Audit Committee
  - Follow up on management action plans to remediate audit issues

---

## 5. Process for Identifying New or Changed Requirements

### 5.1 Regulatory Horizon Scanning

#### 5.1.1 Monitoring Mechanisms
- **Legal & Compliance Team**: Dedicated resources monitor EU and national legislative developments
- **Subscriptions**: Legal databases (LexisNexis, Westlaw), regulatory newsletters, industry associations (EBF, SWIFT, PCI SSC)
- **Regulator Communications**: Monitoring of official communications from:
  - EU institutions (European Commission, EBA, ECB, EDPB)
  - National regulators (BaFin, ACPR, DNB, Banco de España, KNF, CBI)
  - National DPAs (BfDI, CNIL, AP, AEPD, UODO, DPC)
  - National cybersecurity authorities (BSI, ANSSI, CSIRT NASK)
- **Industry Associations**: Participation in European Banking Federation (EBF), national banking associations, FS-ISAC
- **External Legal Counsel**: Engagement of law firms in each country for advisory on legal developments

#### 5.1.2 Horizon Scanning Frequency
- **Daily**: Monitoring of regulatory announcements and official gazettes
- **Weekly**: Internal legal team review of developments
- **Monthly**: Regulatory updates summary prepared by Legal/Compliance team
- **Quarterly**: Regulatory horizon scanning report to Executive Committee and Board Risk Committee

### 5.2 Identification Process

**Step 1: Detection**
- Legal/Compliance team identifies new or amended law, regulation, or regulatory guidance
- Contractual changes identified by Legal Counsel or business units (e.g., contract renewal, new vendor)

**Step 2: Initial Assessment**
- Legal team conducts preliminary analysis:
  - Applicability to EuroTrust Bank AG? (jurisdiction, scope, business activities)
  - Effective date / compliance deadline?
  - Subject matter (data protection, cybersecurity, payments, banking supervision, etc.)?
- If applicable → Proceed to Impact Assessment

**Step 3: Impact Assessment**
- **Cross-functional team** convened: Legal, Compliance, CISO, CRO, DPO, affected business units
- **Assessment questions**:
  - What are the specific obligations?
  - Which systems, processes, business areas are affected?
  - What are the information security implications?
  - Do current controls meet the new requirements, or are gaps identified?
  - What is the remediation effort (time, cost, resources)?
  - What are the consequences of non-compliance (penalties, enforcement actions)?
- **Output**: Impact Assessment Report documenting findings and recommendations

**Step 4: Compliance Plan Development**
- If gaps identified → Develop **Compliance Plan** (also called Remediation Plan or Implementation Plan)
- **Plan includes**:
  - List of actions required (policy updates, control implementations, system changes, training)
  - Responsible owners for each action
  - Timeline and milestones
  - Resource requirements (budget, headcount, vendors)
  - Risk assessment (residual risk if full compliance delayed)
- **Approval**: Compliance Plan approved by Executive Committee (or Board Risk Committee for material changes)

**Step 5: Implementation & Monitoring**
- Business units and support functions execute Compliance Plan
- Compliance team monitors progress (monthly updates)
- Escalation if delays or issues arise

**Step 6: Validation & Documentation**
- Upon completion, Compliance team validates compliance (testing, evidence review)
- Update **Requirements Register** (add new requirement)
- Update policies, procedures, and training materials
- Communicate to relevant stakeholders (employees, Board, regulators if required)

### 5.3 Example: NIS2 Directive Implementation Process (2024-2026)

- **Q4 2022**: NIS2 Directive adopted by EU → Legal team identifies and flags
- **Q1 2023**: Impact Assessment initiated by CCO, CISO, Legal
- **Q2 2023**: Gap Analysis completed (comparing existing controls to NIS2 requirements)
- **Q3 2023**: Compliance Plan developed (actions: policy updates, incident reporting procedures, governance enhancements, training)
- **Q4 2023**: Executive Committee approves Compliance Plan and budget
- **2024**: National transpositions monitored; Compliance Plan execution (aligned with national implementations in Germany, France, NL, Spain, Poland, Ireland)
- **Q1 2025-Q4 2025**: Remediation activities; country-specific updates as national laws finalized
- **Q1 2026**: Validation and ongoing monitoring

---

## 6. Monitoring and Review Procedures

### 6.1 Ongoing Compliance Monitoring

#### 6.1.1 Compliance Monitoring Activities
- **First Line Self-Assessments**: Business units conduct quarterly self-assessments of compliance with key requirements
- **Second Line Reviews**: Compliance, CISO, DPO teams conduct periodic reviews (frequency based on risk and regulatory requirement)
  - **Example**: Quarterly access reviews (BAIT, IAM requirements)
  - **Example**: Annual PCI DSS self-assessment and QSA audit
  - **Example**: Annual SWIFT CSP attestation
- **Key Risk Indicators (KRIs)**: Dashboards tracking compliance metrics (e.g., number of unpatched vulnerabilities, incidents, training completion rates, data breach notification timelines)
- **Incident Monitoring**: All incidents reviewed for potential compliance breaches (regulatory notification obligations, contractual breaches)
- **Regulator Inspections**: Hosting of on-site inspections and reviews by BaFin, ECB, national authorities
- **Third-Party Audits**: External audits (ISO 27001 certification audits, PCI DSS QSA, independent SWIFT CSP assessor)

#### 6.1.2 Compliance Testing
- **Design Testing**: Confirm policies and procedures exist and are documented
- **Operating Effectiveness Testing**: Confirm controls are functioning as designed (e.g., sample testing of access requests, penetration testing, DR testing)
- **Penetration Testing**: Annual external penetration tests (DORA, PSD2, PCI DSS); TLPT every 3 years
- **Disaster Recovery Testing**: Annual DR tests (DORA, EBA Guidelines, BAIT)
- **Internal Audits**: Internal Audit conducts risk-based audits (annual audit plan)

### 6.2 Compliance Reporting

#### 6.2.1 Internal Reporting
- **Monthly**:
  - Information Security Council (CISO-led): Security metrics, incidents, compliance status
  - Compliance Committee (CCO-led): Regulatory developments, compliance issues, action plans
  - Enterprise Risk Committee (CRO-led): IT risk and operational risk metrics
  - Data Protection Forum (DPO-led): GDPR compliance, DPIAs, DSARs

- **Quarterly**:
  - **Executive Committee**: Compliance Dashboard (summary of compliance status across all requirements; KRIs; incidents; regulatory developments)
  - **Board Risk Committee**: Comprehensive compliance report (CCO + CISO presentation)
    - Status of major compliance programs (DORA, NIS2, ISO 27001)
    - Material incidents and breaches
    - Regulatory interactions and inspections
    - Audit findings and remediation status
    - Changes to Requirements Register

- **Annually**:
  - **Board of Directors**: Annual Compliance Report (comprehensive review of compliance with all legal, regulatory, and contractual requirements)
  - **Annual Certification**: CEO and CFO certify to Board that adequate compliance systems are in place

#### 6.2.2 External Reporting (to Regulators)
- **Regulatory Notifications**: As required by law (GDPR breach notifications within 72 hours, DORA incident reports, NIS2 incident reports, PSD2 incident reports, country-specific reporting)
- **Periodic Regulatory Returns**: Submission of required reports (e.g., BaFin MaRisk compliance attestation, SWIFT CSP attestation to correspondents)
- **Supervisory Reviews**: Participation in SREP (Supervisory Review and Evaluation Process) by ECB; national supervisory reviews by BaFin, ACPR, DNB, etc.
- **Certification Audits**: ISO 27001 surveillance audits (annually), PCI DSS QSA audits (annually)

### 6.3 Requirements Register Maintenance

- **Ownership**: Chief Compliance Officer (CCO)
- **Maintenance Process**:
  - New requirement identified → Impact Assessment → Add to Requirements Register (assign Req ID, populate all fields)
  - Requirement amended → Update Requirements Register (reference, obligations, deadlines)
  - Requirement superseded or repealed → Mark as obsolete in Requirements Register
- **Review Frequency**: Quarterly full review of Requirements Register (CCO + Legal + CISO + DPO)
- **Version Control**: Requirements Register versioned and change log maintained

### 6.4 Policy and Procedure Reviews

- **Policy Review Schedule**: All policies reviewed at least annually (or upon regulatory change)
- **Examples**:
  - **Information Security Policy**: Annual review (Board approval)
  - **Data Protection Policy**: Annual review (DPO + Board approval)
  - **Incident Response Policy**: Annual review (CISO)
  - **Third-Party Risk Management Policy**: Annual review (CRO)
- **Procedure Reviews**: Procedures reviewed when regulatory requirements change or after significant incidents (lessons learned)

---

## 7. Integration with the Information Security Management System (ISMS)

EuroTrust Bank AG's compliance approach is **fully integrated with the ISMS** (based on ISO/IEC 27001:2022):

### 7.1 ISMS Scope
- **ISMS Scope**: All information assets, systems, and processes supporting EuroTrust Bank AG's operations across all six European countries
- **ISO 27001 Certification Target**: Q4 2026 (external certification audit)

### 7.2 ISMS Integration Points

#### 7.2.1 Context of the Organization (ISO 27001 Clause 4)
- **Clause 4.1 — Understanding the organization and its context**: Documented in Firm Overview (including business operations, IT infrastructure, regulatory landscape)
- **Clause 4.2 — Understanding the needs and expectations of interested parties**: Stakeholder analysis includes regulators, customers, shareholders, employees
- **Clause 4.3 — Determining the scope of the ISMS**: ISMS scope encompasses all systems subject to legal, regulatory, and contractual requirements

#### 7.2.2 Leadership (ISO 27001 Clause 5)
- **Clause 5.1 — Leadership and commitment**: Board and Executive Committee oversight of ISMS and compliance
- **Clause 5.2 — Policy**: Information Security Policy approved by Board; aligned with regulatory requirements (GDPR Art. 32, DORA, BAIT, EBA Guidelines, etc.)
- **Clause 5.3 — Organizational roles, responsibilities, and authorities**: Roles defined in this Compliance Approach document

#### 7.2.3 Planning (ISO 27001 Clause 6)
- **Clause 6.1.1 — General (Risk Assessment)**: IT risk assessments include legal, regulatory, and contractual compliance risks
- **Clause 6.1.2 — Information security risk assessment**: Risk assessment methodology considers regulatory penalties and contractual liabilities
- **Clause 6.1.3 — Information security risk treatment**: Risk treatment plans include compliance actions (e.g., implement controls to meet GDPR Art. 32, PCI DSS Requirements, SWIFT CSP controls)
- **Clause 6.2 — Information security objectives**: ISMS objectives include compliance objectives (e.g., "Achieve full DORA compliance by Q4 2025")

#### 7.2.4 Support (ISO 27001 Clause 7)
- **Clause 7.2 — Competence**: Training programs include legal, regulatory, and contractual requirements (GDPR training, PCI DSS training, SWIFT CSP awareness)
- **Clause 7.3 — Awareness**: Security awareness training covers regulatory obligations (phishing awareness for GDPR, insider threat for banking regulations)
- **Clause 7.4 — Communication**: Communication plan includes regulatory notifications (incident reporting to DPAs, BSI, SWIFT, etc.)
- **Clause 7.5 — Documented information**: Requirements Register, policies, procedures, evidence of compliance documented and controlled

#### 7.2.5 Operation (ISO 27001 Clause 8)
- **Clause 8.1 — Operational planning and control**: Operational processes aligned with regulatory requirements (e.g., GDPR-compliant data processing, PCI DSS-compliant card processing)
- **Clause 8.2 — Information security risk assessment**: Regular risk assessments (DPIA for GDPR, IT risk assessments per EBA Guidelines)
- **Clause 8.3 — Information security risk treatment**: Controls implemented to meet legal, regulatory, and contractual obligations (see Annex A controls)

#### 7.2.6 Performance Evaluation (ISO 27001 Clause 9)
- **Clause 9.1 — Monitoring, measurement, analysis, and evaluation**: Compliance monitoring (KRIs, compliance dashboards, testing)
- **Clause 9.2 — Internal audit**: Internal Audit audits compliance with legal, regulatory, and contractual requirements
- **Clause 9.3 — Management review**: Board Risk Committee and Executive Committee review compliance performance quarterly

#### 7.2.7 Improvement (ISO 27001 Clause 10)
- **Clause 10.1 — Nonconformity and corrective action**: Non-compliance identified → Root cause analysis → Corrective action plan → Implementation → Validation
- **Clause 10.2 — Continual improvement**: Lessons learned from incidents, audits, and regulatory inspections integrated into ISMS and compliance framework

### 7.3 ISO 27001 Annex A Controls Mapped to Legal, Regulatory, and Contractual Requirements

**Examples**:
- **A.5.31 — Legal, statutory, regulatory and contractual requirements** (THIS DOCUMENT): Documents requirements and approach
- **A.5.2 — Information security roles and responsibilities**: Mapped to roles in Section 4 of this document
- **A.5.10 — Acceptable use of information and other associated assets**: Aligned with GDPR data minimization, BAIT least privilege
- **A.5.29 — Information security during disruption**: Aligned with DORA BCP/DR, EBA Guidelines, BAIT
- **A.5.33 — Records management**: Aligned with GDPR retention (Art. 5), MiFID II record-keeping (5 years), PCI DSS log retention (1 year)
- **A.5.34 — Privacy and protection of PII**: Full GDPR compliance program
- **A.8.9 — Configuration management**: Aligned with BAIT, PCI DSS (hardening, secure configurations)
- **A.8.10 — Information deletion**: Aligned with GDPR right to erasure (Art. 17), data retention limits
- **A.8.16 — Monitoring activities**: Aligned with DORA logging, PCI DSS Requirement 10, BAIT logging
- **A.8.24 — Use of cryptography**: Aligned with GDPR Art. 32, DORA, NIS2, BAIT, PCI DSS (encryption standards)

---

## 8. Training and Awareness

### 8.1 Training Programs

#### 8.1.1 General Compliance & Information Security Training (Mandatory for All Employees)
- **Frequency**: Annually
- **Topics**:
  - Introduction to EuroTrust Bank AG's compliance obligations
  - Information security basics (CIA triad, password security, phishing awareness)
  - **GDPR awareness**: Data protection principles, data subject rights, breach notification
  - **PSD2 awareness**: Strong customer authentication, fraud prevention
  - **Incident reporting**: How to report security incidents
  - **Acceptable use**: IT usage policies, email and internet policies
- **Format**: E-learning (1 hour), mandatory completion tracked
- **Completion Rate Target**: 100% annually (KRI)

#### 8.1.2 Role-Based Compliance Training

##### Information Security Team
- **Topics**: DORA, NIS2, BAIT, EBA ICT Guidelines, ECB cyber resilience expectations, PCI DSS, SWIFT CSP
- **Frequency**: Quarterly updates (regulatory changes), annual comprehensive training
- **Format**: Instructor-led training, external certifications (CISSP, CISM, CISA)

##### Compliance Team
- **Topics**: GDPR, PSD2, AMLD, MiFID II, ePrivacy, national data protection laws, regulatory reporting
- **Frequency**: Quarterly regulatory updates
- **Format**: Instructor-led training, external certifications (CIPP/E, CIPM for data privacy professionals)

##### Data Protection Team
- **Topics**: GDPR deep dive, DPIAs, DSARs, breach notification, national data protection laws
- **Frequency**: Semi-annually (regulatory developments)
- **Format**: Instructor-led training, external certifications (CIPP/E, CIPM)

##### IT and Development Teams
- **Topics**: Secure development (OWASP), data protection by design (GDPR Art. 25), PCI DSS secure coding, SWIFT CSP controls
- **Frequency**: Annually (secure coding), ad-hoc for new technologies
- **Format**: Hands-on workshops, e-learning

##### Payments and Treasury Teams
- **Topics**: PCI DSS (card data handling), SWIFT CSP, PSD2 SCA, sanctions screening
- **Frequency**: Annually
- **Format**: Instructor-led training

##### Country Managers and Country Teams
- **Topics**: Country-specific legal and regulatory requirements (BDSG & BAIT for Germany, LPM for France, DNB Guidelines for Netherlands, etc.)
- **Frequency**: Annually (or upon regulatory change)
- **Format**: Instructor-led training by local Legal/Compliance teams

#### 8.1.3 Executive and Board Training
- **Topics**: Regulatory landscape, DORA, NIS2, cyber risk governance, incident response, Board's role in oversight
- **Frequency**: Semi-annually (Board training session)
- **Format**: Executive briefings, external speakers (e.g., regulators, law firms)

### 8.2 Awareness Campaigns

- **Phishing Simulations**: Quarterly simulated phishing campaigns (measure click rates, provide immediate feedback)
- **Security Awareness Newsletters**: Monthly newsletters covering recent threats, regulatory updates, best practices
- **Posters and Intranet**: Security awareness posters in offices; intranet portal with compliance resources
- **Data Privacy Day** (28 January): Annual awareness campaign focused on GDPR and data protection
- **Cybersecurity Awareness Month** (October): Annual awareness campaign focused on cyber threats and defenses

### 8.3 Training Metrics
- **Completion Rates**: Tracked for all mandatory training (target: 100%)
- **Assessment Scores**: Post-training quizzes (target: 80% pass rate)
- **Phishing Simulation Click Rates**: Track improvement over time (target: <5% click rate)
- **Reporting**: Quarterly training metrics reported to Executive Committee

---

## 9. Record-Keeping and Evidence

### 9.1 Documentation Requirements

To demonstrate compliance with legal, regulatory, and contractual requirements, EuroTrust Bank AG maintains comprehensive documentation:

#### 9.1.1 Governance and Policy Documents
- **Requirements Register** (this document series)
- **Compliance Approach** (this document)
- **Information Security Policy** (Board-approved)
- **Data Protection Policy** (Board-approved)
- **Incident Response Policy**
- **Third-Party Risk Management Policy**
- **Business Continuity Policy**
- **Acceptable Use Policy**
- **Other supporting policies and procedures** (60+ policies and 200+ procedures)

#### 9.1.2 Risk Assessment and Treatment
- **IT Risk Register**: Documented IT risks, assessments, and treatments (aligned with DORA, EBA Guidelines)
- **Data Protection Impact Assessments (DPIAs)**: For high-risk processing activities (GDPR Art. 35)
- **Vendor Risk Assessments**: For all ICT third-party providers (DORA, EBA Outsourcing Guidelines)
- **SWIFT CSP Gap Analysis and Attestation**: Annual self-assessment and attestation

#### 9.1.3 Compliance Evidence
- **Penetration Test Reports**: Annual external penetration tests (DORA, PSD2, PCI DSS)
- **Vulnerability Scan Reports**: Quarterly PCI DSS ASV scans; continuous Qualys scans
- **Disaster Recovery Test Reports**: Annual DR tests (DORA, EBA Guidelines, BAIT)
- **Security Audit Reports**:
  - ISO 27001 certification audit reports (annually once certified)
  - PCI DSS QSA Report on Compliance (ROC) and Attestation of Compliance (AOC) (annually)
  - SWIFT CSP independent assessment report (annually)
  - AWS SOC 2 Type II reports (reviewed annually)
- **Training Records**: Completion of mandatory training (all employees); role-based training (specific teams)
- **Access Review Reports**: Quarterly user access reviews (BAIT Section 4)
- **Incident Reports**: All incidents logged with regulatory notification status
- **Regulatory Correspondence**: Communications with regulators (BaFin, ECB, national DPAs, cybersecurity authorities)

#### 9.1.4 Contractual Evidence
- **Contracts Repository**: All contracts with third parties (cloud, outsourcing, NDAs, etc.)
- **Data Processing Agreements (DPAs)**: With AWS, SaaS vendors, processors (GDPR Art. 28)
- **Standard Contractual Clauses (SCCs)**: For international data transfers
- **Audit Reports from Vendors**: SOC 2, ISO 27001 certificates from critical vendors

### 9.2 Record Retention

- **Retention Periods** (based on legal and regulatory requirements):
  - **General Business Records**: 10 years (German commercial law)
  - **Customer Account Records**: 10 years after account closure (KWG)
  - **Transaction Records**: 5 years (AMLD, MiFID II)
  - **Audit Logs**: 1 year online, 3 years archived (PCI DSS); longer for forensic purposes
  - **GDPR Processing Records**: Duration of processing + statute of limitations (typically 5-10 years)
  - **Personal Data Breach Records**: 3 years (GDPR recommendation)
  - **Policies and Procedures**: Current version + 3 years of superseded versions
  - **Training Records**: Duration of employment + 5 years

- **Storage and Access**:
  - **Electronic Records**: Document management system (Microsoft SharePoint, access-controlled)
  - **Audit Evidence**: GRC tool (e.g., ServiceNow GRC module) for centralized evidence repository
  - **Contracts**: Contract management system (access restricted to Legal, Compliance, Procurement)

### 9.3 Evidence for Audits and Inspections

- **Internal Audits**: Internal Audit has access to all documentation and systems
- **External Audits**: Evidence provided to ISO 27001 auditors, PCI DSS QSA, independent SWIFT CSP assessor
- **Regulatory Inspections**: Evidence provided to BaFin, ECB, national DPAs, cybersecurity authorities during supervisory reviews and investigations
- **Process**: Compliance team coordinates evidence collection and presentation; evidence room setup for on-site inspections

---

## 10. Escalation and Incident Response

### 10.1 Compliance Breach Escalation

**Definition of Compliance Breach**: Failure to meet a legal, regulatory, or contractual obligation related to information security.

**Examples**:
- Personal data breach (GDPR)
- Failure to report major incident within required timeline (DORA, NIS2, PSD2)
- Non-compliance with PCI DSS requirements (e.g., failure to remediate vulnerability within 30 days)
- Breach of AWS DPA or contractual SLA
- Unauthorized disclosure of confidential information (NDA breach)

### 10.2 Escalation Process

**Step 1: Detection**
- Compliance breach identified by:
  - First line (business unit) during self-assessment or operations
  - Second line (Compliance, CISO, DPO) during monitoring or testing
  - Third line (Internal Audit) during audit
  - External party (regulator, customer, vendor)

**Step 2: Reporting**
- Report immediately to:
  - Relevant second-line function (Compliance, CISO, DPO, CRO) depending on nature of breach
  - If information security breach → CISO and Incident Response Team
  - If personal data breach → DPO
  - If contractual breach → Legal Counsel

**Step 3: Assessment**
- Second-line function assesses:
  - Severity of breach (minor, moderate, major, critical)
  - Regulatory notification obligations
  - Contractual notification obligations
  - Potential impact (financial, reputational, legal)
  - Root cause (preliminary assessment)

**Step 4: Notification**
- **Internal Notification**:
  - Minor breaches: Notify relevant business unit head and second-line owner
  - Moderate breaches: Notify CRO, CCO, or CISO (as applicable) and Executive Committee member
  - Major/Critical breaches: Notify CEO, CFO, CRO, CCO, CISO, DPO; escalate to Board Risk Committee
- **External Notification** (if required by law or contract):
  - **GDPR**: DPO notifies DPA within 72 hours; notify data subjects if high risk
  - **DORA/NIS2/PSD2**: Compliance Officer notifies regulator within required timeline (24h, 72h, or as specified)
  - **National Laws**: Notify BSI (Germany), CSIRT NASK (Poland), etc.
  - **Contractual**: Notify AWS, SWIFT, correspondents, insurer (as required by contract)

**Step 5: Remediation**
- Root cause analysis (RCA) conducted
- Corrective action plan developed (immediate containment + long-term remediation)
- Responsible owner assigned
- Timeline and milestones established
- Remediation tracked by Compliance/CISO

**Step 6: Lessons Learned**
- Post-incident review conducted
- Lessons learned documented
- Policies, procedures, or controls updated to prevent recurrence
- Training or awareness campaigns if human error identified

**Step 7: Follow-Up**
- Compliance team monitors remediation to completion
- Validation testing to confirm effectiveness of corrective actions
- Closure of breach incident in tracking system
- Report to Executive Committee and Board on resolution

### 10.3 Regulatory Investigation Support

If a compliance breach results in a regulatory investigation or enforcement action:
- **Coordination**: Legal Counsel leads response; Compliance, CISO, DPO provide support
- **Evidence Collection**: Preserve and collect all relevant evidence (logs, documents, emails)
- **Regulator Engagement**: Designated spokespersons (CEO, CCO, Legal Counsel) interface with regulators
- **Remediation Communication**: Proactive communication of remediation efforts to regulator
- **Settlement Negotiations**: Legal Counsel and CCO negotiate settlements or consent orders (if applicable)

---

## 11. Continuous Improvement

### 11.1 Sources of Improvement

1. **Lessons Learned from Incidents**: Post-incident reviews identify control failures or process gaps
2. **Audit Findings**: Internal Audit and external auditor findings drive improvements
3. **Regulatory Feedback**: Supervisory reviews and inspections by BaFin, ECB, DPAs provide feedback on compliance posture
4. **Regulatory Changes**: New or amended laws/regulations trigger compliance enhancements
5. **Industry Best Practices**: Participation in industry forums (EBF, FS-ISAC) and benchmarking against peers
6. **Technology Evolution**: New technologies (e.g., AI, quantum computing) create new compliance considerations

### 11.2 Improvement Initiatives (2026-2028)

1. **ISO 27001:2022 Certification** (Target: Q4 2026): Formalize and certify ISMS, demonstrating compliance with international best practices
2. **Zero Trust Architecture**: Multi-year initiative to enhance security (network segmentation, identity-centric security, continuous verification)
3. **GRC Tool Implementation**: Implement integrated Governance, Risk, and Compliance (GRC) tool (e.g., ServiceNow GRC) for centralized requirements tracking, compliance monitoring, and evidence management
4. **Enhanced Automation**: Automate compliance monitoring and reporting (e.g., automated access reviews, automated vulnerability scanning and reporting, automated policy attestations)
5. **Third-Party Risk Platform**: Implement third-party risk management platform for continuous monitoring of vendor security posture (e.g., BitSight, SecurityScorecard)
6. **Advanced Threat Detection**: Enhance SOC capabilities with SOAR (Security Orchestration, Automation, and Response) and threat hunting
7. **Data Governance Platform**: Implement data governance platform to enhance GDPR compliance (data discovery, classification, lineage, data subject rights automation)

---

## 12. Conclusion

EuroTrust Bank AG has established a comprehensive and systematic approach to identifying, monitoring, and meeting legal, statutory, regulatory, and contractual requirements related to information security. This approach is fully integrated with the firm's Information Security Management System (ISMS) and supported by clear governance structures, defined roles and responsibilities, robust processes, and a culture of compliance.

Through continuous monitoring, regular reviews, training and awareness, and a commitment to continuous improvement, EuroTrust Bank AG ensures that it remains compliant with applicable obligations and responsive to the evolving regulatory landscape.

---

## Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Compliance Team | Initial version for ISO 27001 audit |

---

**END OF DOCUMENT**

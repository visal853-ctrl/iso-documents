# EU-Wide Regulations — Legal & Regulatory Requirements

## Document Control
- **Document ID**: LRR-EU-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal
- **Owner**: Chief Compliance Officer (CCO) & Data Protection Officer (DPO)

---

## 1. Introduction

This document identifies and catalogues **EU-wide legal and regulatory requirements** applicable to EuroTrust Bank AG's information security management system. These requirements arise from EU Regulations and Directives that are directly applicable or transposed across all EU member states where the firm operates.

This document supports **ISO/IEC 27002:2022 Control 5.31** (Legal, statutory, regulatory and contractual requirements).

---

## 2. EU-Wide Regulations Summary

| # | Regulation/Directive | Reference | Applicability | Primary IS Impact |
|---|---------------------|-----------|---------------|-------------------|
| 1 | GDPR | Regulation (EU) 2016/679 | All operations processing personal data | Data protection, privacy, security measures |
| 2 | PSD2 | Directive (EU) 2015/2366 | Payment services | Strong customer authentication, API security |
| 3 | DORA | Regulation (EU) 2022/2554 | All digital/IT operations | ICT risk management, incident reporting |
| 4 | NIS2 Directive | Directive (EU) 2022/2555 | Critical infrastructure (banking) | Cybersecurity measures, incident response |
| 5 | eIDAS | Regulation (EU) No 910/2014 | Electronic identification & trust services | Digital signatures, authentication |
| 6 | EBA Guidelines (ICT) | EBA/GL/2019/04 | ICT & security risk management | IT governance, risk management |
| 7 | ECB/SSM Expectations | Various ECB guides | Banks under ECB supervision | Cyber resilience frameworks |
| 8 | AMLD 5 & 6 | Directives (EU) 2018/843 & 2018/1673 | AML/CFT obligations | Customer due diligence, transaction monitoring |
| 9 | MiFID II | Directive 2014/65/EU | Investment services (wealth mgmt) | Client data protection, record-keeping |
| 10 | ePrivacy Directive | Directive 2002/58/EC | Electronic communications | Cookies, marketing consent, confidentiality |

---

## 3. Detailed Requirements

### 3.1 GDPR (General Data Protection Regulation)

#### 3.1.1 Basic Information
- **Full Name**: General Data Protection Regulation
- **Reference**: Regulation (EU) 2016/679
- **Effective Date**: 25 May 2018
- **Applicability**: All EuroTrust Bank AG operations processing personal data of EU residents across all six countries
- **Enforcement**: National Data Protection Authorities (DPAs) in each member state
- **Maximum Penalties**: Up to €20 million or 4% of global annual turnover (whichever is greater)

#### 3.1.2 Scope
GDPR applies to:
- Processing of customer personal data (retail & corporate customers)
- Employee data processing
- Marketing and communications
- Cross-border data transfers (e.g., to AWS EU regions)

#### 3.1.3 Key Information Security Obligations

##### Article 5: Principles Relating to Processing
- **Lawfulness, fairness, transparency**
- **Purpose limitation**
- **Data minimization**
- **Accuracy**
- **Storage limitation**
- **Integrity and confidentiality** (security principle)
- **Accountability**

**IS Impact**: Data classification, retention policies, access controls

##### Article 25: Data Protection by Design and by Default
- Implement appropriate technical and organizational measures
- Pseudonymization and encryption where applicable
- Minimize data processing by default

**IS Impact**: Secure development lifecycle, privacy-enhancing technologies (PETs)

##### Article 32: Security of Processing
- State of the art security measures:
  - Pseudonymization and encryption of personal data
  - Ability to ensure ongoing confidentiality, integrity, availability, and resilience
  - Ability to restore availability and access in the event of incident
  - Regular testing and evaluation of security measures

**IS Impact**: Encryption standards, business continuity, penetration testing, vulnerability management

##### Article 33 & 34: Personal Data Breach Notification
- Notify DPA within 72 hours of becoming aware of a breach
- Notify affected data subjects without undue delay (if high risk to rights and freedoms)

**IS Impact**: Incident response procedures, breach notification processes, logging and monitoring

##### Article 35: Data Protection Impact Assessment (DPIA)
- Conduct DPIA for high-risk processing activities
- Required for large-scale systematic monitoring, automated decision-making, sensitive data

**IS Impact**: Risk assessment procedures, privacy impact assessments integrated with ISMS

##### Article 44-50: International Data Transfers
- Adequacy decisions, Standard Contractual Clauses (SCCs), Binding Corporate Rules (BCRs)
- Transfers outside EEA require safeguards

**IS Impact**: AWS data residency controls, SCCs with vendors, data localization requirements

#### 3.1.4 Relevant Articles/Sections
- **Chapter II (Articles 5-11)**: Principles & Lawful Basis
- **Chapter III (Articles 12-23)**: Data Subject Rights
- **Chapter IV (Articles 24-43)**: Controller & Processor Responsibilities
- **Chapter V (Articles 44-50)**: Data Transfers
- **Chapter VII (Articles 82-84)**: Liability & Penalties

#### 3.1.5 Compliance Status
- **Status**: Compliant (ongoing)
- **Last Review**: January 2026
- **Next Review**: July 2026
- **DPO Appointed**: Dr. Sabine Weber

#### 3.1.6 Responsible Department/Role
- **Primary Owner**: Data Protection Officer (DPO)
- **Supporting**: CISO, Compliance, Legal, IT
- **Governance**: Data Protection Working Group (quarterly meetings)

---

### 3.2 PSD2 (Payment Services Directive 2)

#### 3.2.1 Basic Information
- **Full Name**: Payment Services Directive 2 (Revised Payment Services Directive)
- **Reference**: Directive (EU) 2015/2366
- **Transposition Deadline**: 13 January 2018
- **Applicability**: All payment services provided by EuroTrust Bank AG (account information, payment initiation, card-based payments)
- **Enforcement**: National competent authorities (e.g., BaFin, ACPR, DNB)
- **Supplemented by**: EBA Regulatory Technical Standards on Strong Customer Authentication (RTS on SCA)

#### 3.2.2 Scope
- Payment accounts (current accounts)
- Card payments (debit & credit cards)
- Open banking APIs (account information services, payment initiation services)
- Cross-border Euro payments

#### 3.2.3 Key Information Security Obligations

##### Article 95: Strong Customer Authentication (SCA)
- **Requirement**: Multi-factor authentication for electronic payments and access to online banking
- **Elements**: Two or more independent factors from:
  - Knowledge (something the user knows — password, PIN)
  - Possession (something the user has — phone, token)
  - Inherence (something the user is — biometrics)
- **Exemptions**: Low-value transactions (<€30), trusted beneficiaries, low-risk transactions (based on transaction monitoring)

**IS Impact**: MFA implementation, biometric authentication (mobile app), transaction risk analysis

##### Article 96: Protection of Payment Service Users' Credentials
- Secure authentication credentials
- Protection against unauthorized use
- Measures to prevent, detect, and block fraudulent payment transactions

**IS Impact**: Credential storage (hashing, encryption), fraud detection systems, security monitoring

##### Article 97: Incident Reporting
- Notify national competent authority of major operational or security incidents
- Report within defined timelines
- Notify payment service users if incident affects financial interests

**IS Impact**: Incident classification criteria, incident reporting procedures to regulators

##### Article 98: Review and Assessment
- Regular operational and security risk assessments
- Security audits by independent experts at least annually

**IS Impact**: Penetration testing, security audits, third-party assessments

#### 3.2.4 EBA RTS on SCA & Secure Communication
- **Reference**: Commission Delegated Regulation (EU) 2018/389
- **Effective**: 14 September 2019 (with transition periods)
- **Key Provisions**:
  - Dynamic linking of authentication to transaction amount and payee
  - Common and secure communication standards for API-based open banking (OAuth 2.0, OpenID Connect)
  - Exemptions to SCA (transaction risk analysis requirements)

**IS Impact**: API security (OAuth 2.0), dynamic authentication codes, secure channels (TLS 1.2+)

#### 3.2.5 Relevant Articles/Sections
- **Title IV (Articles 66-97)**: Transparency and Information Requirements
- **Chapter 4 (Articles 95-98)**: Security and Operational Requirements

#### 3.2.6 Compliance Status
- **Status**: Compliant
- **Last Review**: December 2025
- **Next Review**: June 2026
- **SCA Implementation**: Completed (2019)

#### 3.2.7 Responsible Department/Role
- **Primary Owner**: Head of Payments & Digital Banking
- **Supporting**: CISO, Compliance, IT Security
- **Regulator Interface**: Compliance Officer (reporting to BaFin, ACPR, DNB, etc.)

---

### 3.3 DORA (Digital Operational Resilience Act)

#### 3.3.1 Basic Information
- **Full Name**: Regulation on Digital Operational Resilience for the Financial Sector
- **Reference**: Regulation (EU) 2022/2554
- **Date of Entry into Force**: 16 January 2023
- **Date of Application**: **17 January 2025** (mandatory compliance)
- **Applicability**: All financial entities, including credit institutions (banks) operating in the EU
- **Enforcement**: National competent authorities + EBA/ECB coordination

#### 3.3.2 Scope
DORA applies to all ICT (Information and Communication Technology) systems, processes, and third-party dependencies supporting EuroTrust Bank AG's operations.

#### 3.3.3 Key Information Security Obligations

##### Article 6: ICT Risk Management Framework
- Establish, maintain, and review a comprehensive ICT risk management framework
- Documented policies, procedures, protocols for ICT risk management
- Address:
  - ICT asset identification and protection
  - ICT incident detection, prevention, response, recovery
  - ICT business continuity and disaster recovery
  - ICT security awareness and training

**IS Impact**: Formalization of IT risk management, asset inventory, cybersecurity policies

##### Article 9-13: ICT-Related Incident Management
- Incident detection, logging, categorization, and escalation
- **Major incident reporting** to competent authority (no later than prescribed timelines)
- Root cause analysis and lessons learned
- Communication to clients and counterparties if necessary

**IS Impact**: Incident response plan, incident classification matrix, regulatory reporting templates

##### Article 17: Testing of ICT Systems
- Conduct testing annually, including:
  - Vulnerability assessments and scans
  - Open source and proprietary software analyses
  - Network security assessments
  - Penetration testing (for critical systems)
  - **Advanced testing**: Threat-led penetration testing (TLPT) every 3 years for significant institutions

**IS Impact**: Annual penetration testing, TLPT program, remediation tracking

##### Article 19-26: ICT Third-Party Risk Management
- Maintain register of all ICT third-party service providers
- Contractual arrangements including:
  - Service level agreements (SLAs)
  - Right to audit
  - Security obligations
  - Incident notification requirements
  - Exit strategies
- **Critical ICT third-party providers** subject to oversight by competent authorities

**IS Impact**: Vendor risk management program, third-party audit rights, contract reviews

##### Article 28-29: ICT Third-Party Provider Oversight
- Financial entities must assess and manage concentration risk to critical ICT providers
- Notification of contractual arrangements with critical providers to authorities

**IS Impact**: Critical vendor identification, concentration risk assessment (e.g., AWS), notification procedures

#### 3.3.4 Relevant Articles/Sections
- **Chapter II (Articles 5-16)**: ICT Risk Management
- **Chapter III (Articles 17-27)**: ICT-Related Incident Management, Classification, and Reporting
- **Chapter IV (Articles 28-44)**: Digital Operational Resilience Testing
- **Chapter V (Articles 28-44)**: Managing ICT Third-Party Risk

#### 3.3.5 Compliance Status
- **Status**: In Progress (mandatory deadline: 17 January 2025 — passed, ongoing compliance)
- **Gap Analysis**: Completed (Q4 2024)
- **Remediation Plan**: In execution (Q1-Q4 2026)
- **Next Review**: April 2026

#### 3.3.6 Responsible Department/Role
- **Primary Owner**: Chief Information Security Officer (CISO)
- **Supporting**: Chief Risk Officer (CRO), IT, Compliance
- **Steering Committee**: DORA Compliance Steering Committee (monthly meetings)
- **Regulator Interface**: Compliance Officer (ECB/BaFin reporting)

---

### 3.4 NIS2 Directive (Network and Information Security Directive 2)

#### 3.4.1 Basic Information
- **Full Name**: Directive on Measures for a High Common Level of Cybersecurity Across the Union
- **Reference**: Directive (EU) 2022/2555 (NIS2 Directive)
- **Adoption**: 14 December 2022
- **Transposition Deadline**: 17 October 2024 (member states must transpose into national law)
- **Applicability**: Credit institutions (including EuroTrust Bank AG) are classified as **Essential Entities** under Annex I
- **Enforcement**: National cybersecurity authorities (CSIRTs, NCAs)

#### 3.4.2 Scope
- Cybersecurity risk management measures
- Network and information system security
- Incident handling and reporting
- Supply chain security

#### 3.4.3 Key Information Security Obligations

##### Article 21: Cybersecurity Risk Management Measures
Essential entities must take appropriate and proportionate technical, operational, and organizational measures to manage cybersecurity risks, including:
- **Risk analysis and information system security policies**
- **Incident handling** (prevention, detection, response, recovery)
- **Business continuity** and crisis management
- **Supply chain security** (security in acquisition, development, maintenance)
- **Security in network and information systems** (access control, asset management)
- **Policies and procedures** for assessing effectiveness of measures
- **Cryptography and encryption** where appropriate
- **Human resources security**, access control, asset management
- **Multi-factor authentication** or continuous authentication
- **Secure voice, video, and text communications** (internal and external)
- **Emergency communication systems**

**IS Impact**: Comprehensive cybersecurity framework, supply chain risk management, encryption policies

##### Article 23: Incident Reporting
Essential entities must notify the relevant CSIRT or national competent authority of:
- **Early warning**: within 24 hours of becoming aware (if significant incident)
- **Incident notification**: within 72 hours (details of incident)
- **Final report**: within 1 month (including impact, response, cross-border implications)

**IS Impact**: Incident reporting timelines, cross-border incident coordination

##### Article 20: Governance
- Management body (board) approves cybersecurity risk management measures
- Management body oversees implementation
- Employees receive cybersecurity training

**IS Impact**: Board-level reporting on cybersecurity, governance documentation

##### Article 32: Supervision and Enforcement
- Ex-ante supervision (audits, on-site inspections)
- Ex-post enforcement (sanctions for non-compliance)

**IS Impact**: Readiness for supervisory audits, documentation of compliance

#### 3.4.4 Penalties
- Administrative fines up to €10 million or 2% of global annual turnover (whichever is higher) for essential entities

#### 3.4.5 Relevant Articles/Sections
- **Chapter IV (Articles 20-23)**: Cybersecurity Risk Management & Incident Reporting
- **Chapter VI (Articles 31-35)**: Supervision and Enforcement

#### 3.4.6 Compliance Status
- **Status**: In Progress (transposition into national laws by October 2024 — monitoring national implementations)
- **Gap Analysis**: Q1 2026 (in progress)
- **Next Review**: July 2026

#### 3.4.7 Responsible Department/Role
- **Primary Owner**: CISO
- **Supporting**: CRO, IT, Compliance
- **National Coordination**: Compliance Officer (coordination with national CSIRTs)

---

### 3.5 eIDAS Regulation (Electronic Identification, Authentication and Trust Services)

#### 3.5.1 Basic Information
- **Full Name**: Regulation on Electronic Identification and Trust Services for Electronic Transactions
- **Reference**: Regulation (EU) No 910/2014
- **Effective Date**: 1 July 2016
- **Applicability**: Electronic identification schemes, electronic signatures, electronic seals, time stamps, electronic registered delivery services
- **Enforcement**: National supervisory bodies
- **Upcoming**: **eIDAS 2.0** (Regulation (EU) 2024/1183) — proposed revisions including European Digital Identity Wallet

#### 3.5.2 Scope
- Electronic signatures used in customer contracts and internal documents
- Trust services for secure communications
- Electronic identification for digital banking (recognition of national eID schemes)

#### 3.5.3 Key Information Security Obligations

##### Article 24: Qualified Electronic Signatures
- Legal effect equivalent to handwritten signature
- Use in loan agreements, account opening documents, wealth management mandates

**IS Impact**: Integration with qualified trust service providers (QTSPs), digital signature workflows

##### Article 19: Security Requirements for Trust Service Providers
- Qualified trust service providers must:
  - Implement security measures to prevent security breaches
  - Notify security breaches to supervisory bodies and affected parties
  - Use trustworthy systems and products
  - Maintain audit logs

**IS Impact**: If EuroTrust Bank issues electronic seals or certificates internally (internal PKI), security compliance with eIDAS requirements

##### Article 9: Mutual Recognition of eID
- Recognize notified electronic identification schemes from other EU member states
- Enable customers from other EU countries to use national eID for authentication

**IS Impact**: Integration of European eID schemes into digital banking authentication (future roadmap under eIDAS 2.0)

#### 3.5.4 Relevant Articles/Sections
- **Chapter II (Articles 6-12)**: Electronic Identification
- **Chapter III (Articles 17-24)**: Trust Services
- **Chapter IV (Articles 25-26)**: Electronic Signatures

#### 3.5.5 Compliance Status
- **Status**: Compliant
- **QTSP Partner**: DigiCert (for document signing)
- **Next Review**: December 2026
- **eIDAS 2.0 Monitoring**: Legal team tracking European Digital Identity Wallet developments

#### 3.5.6 Responsible Department/Role
- **Primary Owner**: Head of Digital Banking
- **Supporting**: IT, Legal, Information Security
- **Trust Services**: Managed by IT Security team

---

### 3.6 EBA Guidelines on ICT and Security Risk Management

#### 3.6.1 Basic Information
- **Full Name**: EBA Guidelines on ICT and Security Risk Management
- **Reference**: EBA/GL/2019/04
- **Issue Date**: 28 November 2019
- **Application Date**: 30 June 2020
- **Applicability**: Credit institutions and investment firms across the EU
- **Status**: Soft law (comply or explain basis)

#### 3.6.2 Scope
- Governance and organization of ICT risk
- ICT risk assessment
- ICT security measures
- ICT third-party risk management
- ICT business continuity management

#### 3.6.3 Key Information Security Obligations

##### Section 4.1: ICT Risk Governance and Strategy
- Management body approves ICT strategy and risk appetite
- Clear roles and responsibilities for ICT risk management
- Segregation of duties

**IS Impact**: ICT governance framework, risk appetite statement, RACI matrix

##### Section 4.2: ICT Risk Assessment
- Comprehensive risk assessment covering all ICT systems
- Regular reviews and updates (at least annually)

**IS Impact**: IT risk assessment methodology, risk register

##### Section 5: ICT Security
- **Section 5.1**: Information security policies (CIA triad)
- **Section 5.2**: Cryptography and encryption
- **Section 5.3**: Network security
- **Section 5.4**: Identity and access management
- **Section 5.5**: Security monitoring and logging
- **Section 5.6**: Physical security of ICT infrastructure

**IS Impact**: Information security policies aligned with EBA guidelines, encryption standards, IAM policies

##### Section 6: ICT Third-Party Risk Management
- Due diligence on ICT third-party providers
- Contractual arrangements with security clauses
- Ongoing monitoring of third parties

**IS Impact**: Vendor risk management framework, contract templates

##### Section 7: ICT Business Continuity Management
- ICT business continuity plans and disaster recovery plans
- Regular testing (at least annually)
- Recovery time objectives (RTO) and recovery point objectives (RPO)

**IS Impact**: BCP/DR documentation, DR testing schedule

#### 3.6.4 Compliance Status
- **Status**: Compliant
- **Last Assessment**: June 2025
- **Next Review**: June 2026

#### 3.6.5 Responsible Department/Role
- **Primary Owner**: CISO
- **Supporting**: CRO, IT
- **Governance**: ICT Risk Committee (quarterly)

---

### 3.7 ECB/SSM Supervisory Expectations on Cyber Resilience

#### 3.7.1 Basic Information
- **Full Name**: ECB Guide on Cyber Resilience Expectations for Financial Market Infrastructures
- **Reference**: ECB Cyber Resilience Oversight Expectations (CROE)
- **Applicability**: Significant institutions under SSM (Single Supervisory Mechanism) supervision, including EuroTrust Bank AG
- **Status**: Supervisory expectations (not legally binding but used in SREP assessments)

#### 3.7.2 Scope
- Cyber resilience strategy
- Governance of cyber risk
- Cyber threat intelligence
- Vulnerability and patch management
- Penetration testing
- Incident response and cyber crisis management

#### 3.7.3 Key Supervisory Expectations

##### Governance
- Board oversight of cyber resilience
- Clear accountability for cyber risk management
- Cyber resilience framework aligned with overall risk management

**IS Impact**: Board reporting on cyber risk, cyber risk governance charter

##### Threat Intelligence
- Establish threat intelligence capability
- Participation in information-sharing initiatives (e.g., financial sector ISACs)

**IS Impact**: Threat intelligence function, membership in FS-ISAC (Financial Services Information Sharing and Analysis Center)

##### Testing
- Regular penetration testing
- Red teaming exercises
- TLPT (Threat-Led Penetration Testing) framework participation

**IS Impact**: Penetration testing program, TLPT exercises

##### Incident Response
- Cyber incident response plan
- Crisis management procedures
- Regular testing of incident response capabilities

**IS Impact**: Cyber incident response playbooks, tabletop exercises

#### 3.7.4 Compliance Status
- **Status**: Compliant (ongoing)
- **Last SREP Assessment**: 2025
- **TLPT Exercise**: Scheduled Q3 2026

#### 3.7.5 Responsible Department/Role
- **Primary Owner**: CISO
- **Supporting**: CRO, Board Risk Committee
- **ECB Interface**: CRO (SREP process)

---

### 3.8 EU Anti-Money Laundering Directives (AMLD 5 & 6)

#### 3.8.1 Basic Information
- **AMLD 5**: Directive (EU) 2018/843 (Fifth Anti-Money Laundering Directive)
- **AMLD 6**: Directive (EU) 2018/1673 (Directive on combating money laundering by criminal law)
- **Effective Dates**: AMLD 5 transposition by 10 January 2020; AMLD 6 transposition by 3 December 2020
- **Applicability**: Obliged entities including credit institutions
- **Enforcement**: National Financial Intelligence Units (FIUs), financial supervisors

#### 3.8.2 Scope
- Customer due diligence (CDD) and enhanced due diligence (EDD)
- Transaction monitoring
- Suspicious activity reporting (SARs)
- Record-keeping
- Internal controls and training

#### 3.8.3 Key Information Security Obligations

##### AMLD 5 — Article 32: Internal Policies, Controls, and Procedures
- Risk management systems including:
  - Customer due diligence
  - Reporting of suspicious transactions
  - Record retention (5 years)
  - **Data protection** when processing personal data for AML purposes
  - Employee screening

**IS Impact**: AML transaction monitoring systems, secure customer data storage, access controls for AML data

##### AMLD 5 — Beneficial Ownership Registries
- Access to national beneficial ownership registers
- Verification of customer beneficial ownership

**IS Impact**: Integration with national UBO registers, data exchange security

##### AMLD 6 — Enhanced Criminalization
- Harmonized definition of money laundering offenses
- Increased penalties
- Extended statute of limitations

**IS Impact**: Incident response for suspected financial crime, cooperation with law enforcement

#### 3.8.4 Information Security Considerations
- **Transaction Monitoring Systems**: Real-time monitoring of payment transactions for suspicious patterns
- **Secure Data Storage**: Customer identification documents, transaction records (5-year retention)
- **Access Controls**: Restricted access to AML data (need-to-know principle)
- **Audit Trails**: Logging and monitoring of access to AML systems

#### 3.8.5 Relevant Articles/Sections
- **AMLD 5 — Chapter II (Articles 13-24)**: Customer Due Diligence
- **AMLD 5 — Chapter III (Articles 30-44)**: Reporting Obligations, Internal Controls

#### 3.8.6 Compliance Status
- **Status**: Compliant
- **Last Review**: October 2025
- **Next Review**: April 2026
- **MLRO (Money Laundering Reporting Officer)**: Designated

#### 3.8.7 Responsible Department/Role
- **Primary Owner**: Chief Compliance Officer (CCO) / MLRO
- **Supporting**: IT, Information Security, Legal
- **System Owner**: AML Transaction Monitoring System Owner

---

### 3.9 MiFID II (Markets in Financial Instruments Directive II)

#### 3.9.1 Basic Information
- **Full Name**: Directive 2014/65/EU (Markets in Financial Instruments Directive II)
- **Supplemented by**: Regulation (EU) No 600/2014 (MiFIR — Markets in Financial Instruments Regulation)
- **Effective Date**: 3 January 2018
- **Applicability**: Investment services provided by EuroTrust Bank AG's wealth management division
- **Enforcement**: National competent authorities (e.g., BaFin, ACPR, AFM)

#### 3.9.2 Scope
- Investment services and activities (portfolio management, investment advice, execution of orders)
- Client asset protection
- Conduct of business rules
- Record-keeping

#### 3.9.3 Key Information Security Obligations

##### Article 16(6): Organizational Requirements
- Firms must maintain systems and procedures to safeguard the security, integrity, and confidentiality of information
- Business continuity arrangements

**IS Impact**: Information security controls for investment systems, BCP/DR plans

##### Article 16(5): Record-Keeping
- Retain records of services and transactions (minimum 5 years)
- Records must be accessible to competent authorities

**IS Impact**: Secure archival of investment records, audit trails, data retention policies

##### MiFIR Article 26: Obligation to Report Transactions
- Transaction reporting to competent authorities
- Data integrity and completeness

**IS Impact**: Transaction reporting systems, data quality controls

##### Commission Delegated Regulation (EU) 2017/565 — Article 23: Algorithmic Trading
- Resilience of trading systems
- System testing and monitoring
- Business continuity arrangements

**IS Impact**: Trading system resilience, change management for algorithmic trading systems

#### 3.9.4 Relevant Articles/Sections
- **MiFID II — Chapter II (Articles 16-20)**: Organizational Requirements
- **MiFID II — Chapter III (Articles 24-30)**: Conduct of Business Rules
- **MiFIR — Article 26**: Transaction Reporting

#### 3.9.5 Compliance Status
- **Status**: Compliant
- **Applicable Division**: Wealth Management
- **Last Review**: September 2025
- **Next Review**: March 2026

#### 3.9.6 Responsible Department/Role
- **Primary Owner**: Head of Wealth Management
- **Supporting**: Compliance, IT, Information Security
- **Regulator Interface**: Compliance Officer

---

### 3.10 ePrivacy Directive

#### 3.10.1 Basic Information
- **Full Name**: Directive 2002/58/EC (Directive on Privacy and Electronic Communications)
- **Reference**: Directive 2002/58/EC (as amended by Directive 2009/136/EC)
- **Effective Date**: 31 July 2002 (amended 25 May 2011)
- **Applicability**: Electronic communications, online services, cookies, direct marketing
- **Enforcement**: National data protection authorities
- **Status**: **ePrivacy Regulation** (proposed replacement for Directive) — under negotiation (not yet adopted)

#### 3.10.2 Scope
- Confidentiality of electronic communications
- Use of cookies and similar tracking technologies
- Unsolicited electronic marketing (email, SMS)
- Traffic and location data

#### 3.10.3 Key Information Security Obligations

##### Article 4: Security of Processing
- Public communications network providers and electronic communications service providers must:
  - Take appropriate technical and organizational measures to safeguard security
  - Notify authority and users of security breaches

**IS Impact**: Security measures for communication services (email, messaging)

##### Article 5: Confidentiality of Communications
- Prohibition of interception or surveillance of communications without user consent
- Exceptions for lawful interception (e.g., law enforcement)

**IS Impact**: Email encryption, secure messaging, access controls on communication systems

##### Article 6: Traffic Data
- Traffic data must be erased or anonymized when no longer needed for transmission
- Processing only for specific purposes (billing, marketing with consent)

**IS Impact**: Data retention policies, log anonymization

##### Article 5(3): Use of Cookies
- Consent required for storing or accessing information on user's device (cookies)
- Exceptions for strictly necessary cookies (e.g., authentication)

**IS Impact**: Cookie consent management on EuroTrust Bank AG website, cookie banners, opt-in mechanisms

##### Article 13: Unsolicited Communications (Direct Marketing)
- Prior consent required for electronic marketing (email, SMS) to individuals
- Opt-out mechanism must be provided

**IS Impact**: Marketing consent management, CRM integration, opt-out handling

#### 3.10.4 Relevant Articles/Sections
- **Article 4**: Security of Processing
- **Article 5**: Confidentiality of Communications & Cookies
- **Article 13**: Unsolicited Communications

#### 3.10.5 Compliance Status
- **Status**: Compliant
- **Cookie Consent Tool**: OneTrust
- **Last Review**: November 2025
- **Next Review**: May 2026
- **ePrivacy Regulation Monitoring**: Legal team tracking EU legislative process

#### 3.10.6 Responsible Department/Role
- **Primary Owner**: Data Protection Officer (DPO)
- **Supporting**: Marketing, IT, Legal
- **Cookie Management**: Digital Marketing Team

---

## 4. Summary of Compliance Responsibilities

| Regulation | Primary Owner | Secondary Owners | Review Frequency |
|------------|---------------|------------------|------------------|
| GDPR | DPO | CISO, Compliance, Legal | Quarterly |
| PSD2 | Head of Payments | CISO, Compliance | Semi-annually |
| DORA | CISO | CRO, IT, Compliance | Quarterly |
| NIS2 | CISO | CRO, Compliance | Quarterly |
| eIDAS | Head of Digital Banking | IT Security, Legal | Annually |
| EBA ICT Guidelines | CISO | CRO | Annually |
| ECB Cyber Expectations | CISO | CRO, Board | Annually (SREP) |
| AMLD 5/6 | CCO / MLRO | Compliance, IT | Semi-annually |
| MiFID II | Head of Wealth Mgmt | Compliance, IT | Annually |
| ePrivacy | DPO | Marketing, IT | Annually |

---

## 5. Cross-Cutting Themes

### 5.1 Encryption & Cryptography
- **Applicable Regulations**: GDPR (Art. 32), DORA, EBA Guidelines, NIS2
- **Requirements**: State-of-the-art encryption for data at rest and in transit
- **Implementation**: AES-256 for data at rest, TLS 1.3 for data in transit

### 5.2 Incident Reporting
- **Applicable Regulations**: GDPR (72 hours), PSD2, DORA, NIS2 (24/72 hours/1 month)
- **Requirements**: Multiple overlapping incident notification obligations
- **Implementation**: Unified incident response process with regulatory mapping

### 5.3 Third-Party Risk Management
- **Applicable Regulations**: DORA (Articles 19-26), EBA Guidelines, NIS2
- **Requirements**: Vendor risk assessment, contractual security clauses, right to audit
- **Implementation**: Centralized vendor risk management program

### 5.4 Business Continuity & Disaster Recovery
- **Applicable Regulations**: DORA, EBA Guidelines, MiFID II, NIS2
- **Requirements**: BCP/DR plans, RTO/RPO definitions, regular testing
- **Implementation**: Enterprise BCP program, annual DR tests

### 5.5 Penetration Testing & Security Assessments
- **Applicable Regulations**: DORA (Art. 17, TLPT), PSD2 (Art. 98), EBA Guidelines, NIS2
- **Requirements**: Annual penetration testing, TLPT for significant institutions
- **Implementation**: Annual external penetration tests, TLPT every 3 years

---

## 6. Regulatory Horizon Scanning

### 6.1 Upcoming Changes
1. **ePrivacy Regulation**: Replacement of ePrivacy Directive (timeline uncertain)
2. **AI Act**: Regulation (EU) 2024/1689 — applicable if AI used in credit scoring, fraud detection
3. **Data Act**: Regulation (EU) 2023/2854 — data sharing obligations (effective 12 September 2025)
4. **Cyber Resilience Act**: Regulation (EU) 2024/2847 — applicable to digital products (ICT systems)
5. **eIDAS 2.0**: European Digital Identity Wallet framework

### 6.2 Monitoring Process
- **Responsibility**: Legal & Compliance teams
- **Frequency**: Monthly regulatory updates
- **Communication**: Quarterly briefings to CISO, CRO, Executive Committee

---

## 7. Document Maintenance

### 7.1 Review Schedule
- **Frequency**: Quarterly
- **Next Scheduled Review**: April 2026
- **Owner**: Chief Compliance Officer

### 7.2 Change Process
- Legislative changes → Legal team analysis → Impact assessment → Compliance plan update → Executive approval

---

## Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Compliance & Legal Teams | Initial version for ISO 27001 audit |

---

**END OF DOCUMENT**

# Country-Specific Regulations — Legal & Regulatory Requirements

## Document Control
- **Document ID**: LRR-CS-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal
- **Owner**: Chief Compliance Officer (CCO) & Legal Counsel

---

## 1. Introduction

This document identifies and catalogues **national and country-specific legal and regulatory requirements** applicable to EuroTrust Bank AG's operations in each of the six European countries where the firm has physical presence: Germany, France, Netherlands, Spain, Poland, and Ireland.

These requirements supplement the EU-wide regulations and reflect national transpositions of EU directives as well as purely domestic legislation related to information security, data protection, banking supervision, and cybersecurity.

This document supports **ISO/IEC 27002:2022 Control 5.31** (Legal, statutory, regulatory and contractual requirements).

---

## 2. Country-Specific Requirements Summary

| Country | Key Regulations | Primary Regulator(s) | Information Security Focus |
|---------|-----------------|---------------------|----------------------------|
| Germany | BDSG, KWG, BAIT, IT-SiG 2.0 | BaFin, BSI, BfDI | Banking IT requirements, data protection, critical infrastructure |
| France | Loi Informatique et Libertés, ACPR Guidelines, LPM | ACPR, CNIL, ANSSI | Data protection, critical infrastructure, operational resilience |
| Netherlands | UAVG, DNB Guidelines | DNB, AP | Data protection, IT risk management |
| Spain | LOPDGDD, Banco de España Circulars | Banco de España, AEPD | Data protection, IT risk, operational continuity |
| Poland | Cybersecurity Act, KNF Guidelines | KNF, UODO, CSIRT NASK | Cybersecurity, data protection, incident reporting |
| Ireland | Data Protection Act 2018, CBI Guidelines | CBI, DPC | Data protection, IT & cyber resilience |

---

## 3. Germany

### 3.1 Overview
As the headquarters jurisdiction, Germany imposes the most comprehensive set of national requirements on EuroTrust Bank AG. German banking supervision under BaFin is among the strictest in Europe, with detailed IT security requirements specific to financial institutions.

---

### 3.2 BDSG (Bundesdatenschutzgesetz — Federal Data Protection Act)

#### 3.2.1 Basic Information
- **Full Name**: Bundesdatenschutzgesetz (Federal Data Protection Act)
- **Reference**: BDSG (2018 version, as amended)
- **Effective Date**: 25 May 2018 (aligned with GDPR)
- **Purpose**: Supplements and specifies GDPR implementation in Germany
- **Enforcement**: BfDI (Federal Commissioner for Data Protection and Freedom of Information), state data protection authorities

#### 3.2.2 Scope
- All processing of personal data by EuroTrust Bank AG in Germany
- Supplements GDPR with German-specific provisions

#### 3.2.3 Key Information Security Obligations

##### Section 22-24: Data Processing by Public Bodies
- Not directly applicable to private bank, but relevant for cooperation with authorities

##### Section 26: Employee Data Processing
- Specific rules for processing employee personal data
- **IS Impact**: HR systems security, employee monitoring limitations

##### Section 64: Data Protection Officer Requirements
- Mandatory DPO if more than 20 persons regularly process personal data (automatically applies to EuroTrust Bank AG)
- **IS Impact**: DPO role formalized, reporting structure

#### 3.2.4 Compliance Status
- **Status**: Compliant
- **Last Review**: January 2026
- **Responsible**: DPO (Dr. Sabine Weber)

---

### 3.3 KWG (Kreditwesengesetz — Banking Act)

#### 3.3.1 Basic Information
- **Full Name**: Kreditwesengesetz (Banking Act)
- **Reference**: KWG (as amended, latest version)
- **Purpose**: Core banking supervision law in Germany
- **Enforcement**: BaFin, Deutsche Bundesbank

#### 3.3.2 Scope
- All banking activities of EuroTrust Bank AG
- Prudential supervision, capital requirements, operational risk

#### 3.3.3 Key Information Security Obligations

##### Section 25a KWG: Organizational Requirements
- Banks must have proper business organization, including:
  - Adequate risk management systems
  - **Adequate internal control mechanisms**
  - **IT systems** that are appropriate, comprehensible, and secure
  - Business continuity management

**IS Impact**: IT governance, risk management framework, internal controls, BCM

##### Section 25b KWG: Outsourcing
- Detailed requirements for outsourcing material banking functions
- Written contracts required
- Right to audit
- Notification to BaFin for material outsourcing

**IS Impact**: Cloud outsourcing to AWS (notification to BaFin), contractual security clauses, audit rights

##### MaRisk (Minimum Requirements for Risk Management)
- BaFin circular implementing Section 25a KWG
- **AT 7.2**: Requirements for outsourcing
- **AT 8**: Business continuity management
- **BTR 3**: Requirements for IT systems and IT operations

**IS Impact**: IT risk management processes aligned with MaRisk, outsourcing register, BCM framework

#### 3.3.4 Compliance Status
- **Status**: Compliant
- **Last BaFin Inspection**: 2025
- **Responsible**: CRO, CISO

---

### 3.4 BAIT (Bankaufsichtliche Anforderungen an die IT — Supervisory Requirements for IT in Financial Institutions)

#### 3.4.1 Basic Information
- **Full Name**: Bankaufsichtliche Anforderungen an die IT (Supervisory Requirements for IT in Financial Institutions)
- **Issuer**: BaFin (Federal Financial Supervisory Authority)
- **Reference**: BAIT (version 2.0, effective 1 August 2021)
- **Purpose**: Concrete supervisory expectations for IT operations and security in banks
- **Enforcement**: BaFin (through supervisory reviews and on-site inspections)

#### 3.4.2 Scope
- **All IT systems** supporting EuroTrust Bank AG's banking operations in Germany
- Includes core banking, payment systems, customer-facing applications, infrastructure

#### 3.4.3 Key Information Security Obligations

##### Section 1: IT Strategy
- Management board must define and approve IT strategy aligned with business strategy
- IT strategy covers IT operations, information security, projects, outsourcing

**IS Impact**: Documented IT strategy, Board approval, annual review

##### Section 2: IT Governance
- Clear responsibilities for IT operations and information security
- Segregation of duties
- IT organization chart

**IS Impact**: IT governance model, RACI matrix, organizational structure

##### Section 3: Information Risk Management and Information Security Management
- Implement information security management system (ISMS) based on recognized standards (ISO 27001)
- Information security policy approved by management board
- Risk assessment of IT systems
- Security incident management

**IS Impact**: ISO 27001 ISMS implementation, information security policy, IT risk register, incident response

##### Section 4: User Access Management
- Identity and access management (IAM) process
- Principle of least privilege
- Segregation of duties in critical functions (e.g., payments)
- Regular access reviews

**IS Impact**: IAM policies, privileged access management, quarterly access reviews

##### Section 5: IT Projects and Development
- Secure software development lifecycle (SDLC)
- Testing before production deployment
- Change management process

**IS Impact**: DevSecOps practices, UAT environments, change approval board

##### Section 6: IT Operations
- Documented IT operations procedures
- Capacity and performance management
- Logging and monitoring
- Patch management

**IS Impact**: ITIL-based IT operations, vulnerability management, SIEM logging

##### Section 7: IT Outsourcing
- Risk assessment before outsourcing
- Written contracts with security and audit clauses
- Notification to BaFin for material outsourcing
- Exit planning

**IS Impact**: Cloud governance for AWS, vendor risk assessments, contract reviews, exit strategies

##### Section 8: Data Backup and Disaster Recovery
- Regular data backups (daily for critical systems)
- Off-site backup storage
- Documented disaster recovery plans
- Annual DR testing

**IS Impact**: Backup policies, Amsterdam DR site, annual DR tests

##### Section 9: Network Management
- Network segmentation
- Secure remote access
- Monitoring and intrusion detection

**IS Impact**: Network architecture, VPN security, IDS/IPS deployment

#### 3.4.4 Compliance Status
- **Status**: Compliant
- **Last Self-Assessment**: December 2025
- **Next Review**: June 2026
- **Responsible**: CISO, CIO

---

### 3.5 IT-SiG 2.0 (IT Security Act 2.0)

#### 3.5.1 Basic Information
- **Full Name**: IT-Sicherheitsgesetz 2.0 (IT Security Act 2.0)
- **Reference**: Act to Increase the Security of Information Technology Systems (IT Security Act 2.0)
- **Effective Date**: 28 May 2021
- **Purpose**: Strengthen cybersecurity for critical infrastructure operators
- **Enforcement**: BSI (Federal Office for Information Security — Bundesamt für Sicherheit in der Informationstechnik)

#### 3.5.2 Scope
- EuroTrust Bank AG qualifies as **critical infrastructure** under the financial sector category
- Applies to IT systems supporting critical banking services

#### 3.5.3 Key Information Security Obligations

##### Section 8a BSIG: Security of Critical Infrastructure
- Implement state-of-the-art technical and organizational measures
- Use IT security products and services that meet state-of-the-art requirements
- Report significant cyber incidents to BSI within **timelines** (as specified)
- Participate in BSI information sharing

**IS Impact**: Advanced security controls, incident reporting to BSI, participation in BSI-CS (Cyber Security) community

##### Section 8b BSIG: Detection Systems for IT Attacks
- Operators of critical infrastructure must implement systems to detect attacks on IT systems
- Report detected attacks to BSI

**IS Impact**: SIEM (Splunk), IDS/IPS, threat detection capabilities, integration with BSI reporting portal

##### Consumer Protection Provisions
- IT-SiG 2.0 introduces consumer notification requirements for certain incidents

**IS Impact**: Customer communication plans for cybersecurity incidents

#### 3.5.4 Compliance Status
- **Status**: Compliant
- **Critical Infrastructure Registration**: Completed with BSI
- **Last Incident Report to BSI**: N/A (no significant incidents in reporting period)
- **Responsible**: CISO

---

### 3.6 Germany Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| BDSG | Federal Data Protection Act | Employee data protection, DPO | DPO | Annually |
| KWG Section 25a/b | Banking Act | IT systems security, outsourcing | CRO, CISO | Ongoing |
| BAIT | BaFin IT Requirements | ISMS, IAM, DR, outsourcing | CISO, CIO | Semi-annually |
| IT-SiG 2.0 | IT Security Act 2.0 | Critical infrastructure security, incident reporting to BSI | CISO | Annually |

---

## 4. France

### 4.1 Overview
France imposes stringent data protection and cybersecurity requirements, particularly for entities considered as operators of vital importance (OIV) under the Military Programming Law (LPM). The ACPR (banking supervisor) also issues detailed guidelines on IT and operational resilience.

---

### 4.2 Loi Informatique et Libertés

#### 4.2.1 Basic Information
- **Full Name**: Loi n° 78-17 du 6 janvier 1978 relative à l'informatique, aux fichiers et aux libertés (Data Protection Act)
- **Reference**: Law No. 78-17 (as amended in 2018 to align with GDPR)
- **Effective Date**: 6 January 1978 (GDPR amendments: 25 May 2018)
- **Purpose**: French implementation of GDPR
- **Enforcement**: CNIL (Commission Nationale de l'Informatique et des Libertés)

#### 4.2.2 Scope
- All processing of personal data by EuroTrust Bank AG's French branches
- Supplements GDPR with French-specific provisions

#### 4.2.3 Key Information Security Obligations

##### Article 32: DPO Requirements
- French banks must appoint a DPO (consistent with GDPR)
- DPO must be registered with CNIL

**IS Impact**: DPO designation for France, reporting to CNIL

##### Chapter V: Specific Processing Activities
- Special regimes for health data, biometric data, criminal records
- Relevant for employee biometric authentication (if implemented)

**IS Impact**: Biometric data governance, CNIL notifications

#### 4.2.4 Compliance Status
- **Status**: Compliant
- **French DPO**: Part of central DPO function (Dr. Sabine Weber) with local liaison in Paris
- **CNIL Registration**: Completed

---

### 4.3 ACPR Guidelines on Operational Resilience and IT Security

#### 4.3.1 Basic Information
- **Full Name**: ACPR Guidelines on Internal Control and Risk Management (including IT risk)
- **Issuer**: ACPR (Autorité de contrôle prudentiel et de résolution)
- **Reference**: Various circulars and guidelines
- **Purpose**: Supervisory expectations for banks' operational resilience
- **Enforcement**: ACPR (on-site inspections, supervisory reviews)

#### 4.3.2 Scope
- IT risk management
- Business continuity
- Outsourcing (cloud services, IT providers)

#### 4.3.3 Key Information Security Obligations

##### IT Governance
- IT strategy aligned with business objectives
- IT risk management framework
- Segregation of duties

**IS Impact**: IT governance documentation, IT risk assessments

##### Business Continuity
- BCP and DR plans for critical functions
- Regular testing (at least annually)
- Recovery objectives (RTO/RPO)

**IS Impact**: France-specific BCP plans, coordination with Paris office DR procedures

##### Outsourcing to Cloud Providers
- Risk assessment before outsourcing
- Contractual security clauses
- ACPR notification for material outsourcing

**IS Impact**: AWS cloud usage notification to ACPR, contract review

#### 4.3.4 Compliance Status
- **Status**: Compliant
- **Last ACPR Inspection**: 2024
- **Responsible**: Country Manager (France), supported by CISO

---

### 4.4 LPM (Loi de Programmation Militaire — Military Programming Law)

#### 4.4.1 Basic Information
- **Full Name**: Loi de Programmation Militaire 2019-2025 (Military Programming Law)
- **Reference**: Law No. 2013-1168 (as updated by LPM 2019-2025)
- **Purpose**: Protection of critical infrastructure and operators of vital importance (OIV)
- **Enforcement**: ANSSI (Agence Nationale de la Sécurité des Systèmes d'Information), Prime Minister's Office

#### 4.4.2 Scope
- **OIV Status**: Major banks may be designated as Operators of Vital Importance
- **EuroTrust Bank AG Status**: Not designated as OIV (size threshold not met), but subject to monitoring

#### 4.4.3 Key Obligations (if designated as OIV)
- Security measures for critical information systems
- Mandatory use of qualified security products (certain categories)
- Incident reporting to ANSSI
- Regular security audits

**IS Impact**: If designated, significant additional security requirements and ANSSI oversight

#### 4.4.4 Compliance Status
- **Status**: Monitored (not currently designated as OIV)
- **ANSSI Engagement**: Voluntary participation in ANSSI threat intelligence sharing
- **Responsible**: CISO, Country Manager (France)

---

### 4.5 France Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| Loi Informatique et Libertés | Law No. 78-17 | Data protection, DPO, CNIL notifications | DPO | Annually |
| ACPR Guidelines | Various circulars | IT governance, BCP, outsourcing | Country Mgr (FR), CISO | Annually |
| LPM | Military Programming Law | Critical infrastructure (if OIV) | CISO | Monitoring |

---

## 5. Netherlands

### 5.1 Overview
The Netherlands has a mature regulatory environment for banking and data protection. DNB (De Nederlandsche Bank) provides detailed guidance on IT and information security risk management. The Netherlands also hosts EuroTrust Bank AG's secondary data centre in Amsterdam.

---

### 5.2 UAVG (Uitvoeringswet AVG — Dutch GDPR Implementation Act)

#### 5.2.1 Basic Information
- **Full Name**: Uitvoeringswet Algemene Verordening Gegevensbescherming (Dutch GDPR Implementation Act)
- **Reference**: UAVG (effective 25 May 2018)
- **Purpose**: National implementation and specification of GDPR in the Netherlands
- **Enforcement**: Autoriteit Persoonsgegevens (AP — Dutch Data Protection Authority)

#### 5.2.2 Scope
- All processing of personal data by EuroTrust Bank AG in the Netherlands
- Includes operations in Amsterdam (including data centre)

#### 5.2.3 Key Information Security Obligations

##### Article 30: Processing by Employers
- Specific rules for employee monitoring and data processing
- Relevant for HR systems and employee access logging

**IS Impact**: Employee monitoring policies, HR systems security

##### Article 41: DPO Requirements
- DPO required for public authorities and certain private organizations
- Banks typically require DPO under GDPR Article 37

**IS Impact**: DPO function covers Netherlands operations

#### 5.2.4 Compliance Status
- **Status**: Compliant
- **AP Registration**: Completed for Dutch operations
- **Responsible**: DPO, supported by Country Manager (Netherlands)

---

### 5.3 DNB Guidelines on IT and Information Security

#### 5.3.1 Basic Information
- **Full Name**: DNB Good Practices on Managing Information Security and Cyber Resilience
- **Issuer**: De Nederlandsche Bank (DNB — Dutch Central Bank)
- **Reference**: Various DNB publications and circulars
- **Purpose**: Supervisory expectations for banks' IT security and cyber resilience
- **Enforcement**: DNB (supervisory reviews, thematic inspections)

#### 5.3.2 Scope
- IT risk management
- Cybersecurity measures
- Outsourcing and third-party risk
- Operational resilience

#### 5.3.3 Key Information Security Obligations

##### Good Practice 1: Governance and Strategy
- Board oversight of IT and cybersecurity risks
- Clear IT strategy and risk appetite
- Three lines of defense model

**IS Impact**: IT governance documentation for Netherlands, Board reporting

##### Good Practice 2: Risk Management
- Regular IT risk assessments
- Integration of IT risk into enterprise risk management
- Scenario analysis and stress testing

**IS Impact**: IT risk register for Netherlands operations, scenario-based risk assessments

##### Good Practice 3: Operational Resilience
- Business continuity and disaster recovery
- **Amsterdam data centre**: Critical role in DR strategy
- Testing of failover procedures

**IS Impact**: Amsterdam DR site operational readiness, DR testing (Frankfurt <-> Amsterdam failover)

##### Good Practice 4: Third-Party Risk Management
- Due diligence on critical IT suppliers
- Concentration risk management (e.g., AWS)
- Exit planning

**IS Impact**: Vendor risk assessments for Netherlands-based suppliers, cloud governance

##### Good Practice 5: Incident Management
- Cyber incident response capabilities
- Incident reporting to DNB (for significant incidents)
- Lessons learned process

**IS Impact**: Incident reporting procedures to DNB, incident playbooks

##### Good Practice 6: Threat Intelligence
- Participation in information sharing (e.g., financial sector ISACs)
- Integration of threat intelligence into security operations

**IS Impact**: Threat intelligence subscriptions, participation in Dutch banking sector ISAC

#### 5.3.4 Compliance Status
- **Status**: Compliant
- **Last DNB Review**: 2025
- **Amsterdam Data Centre**: Tier III certified, compliant with DNB expectations
- **Responsible**: Country Manager (Netherlands), CISO

---

### 5.4 Wet Beveiliging Netwerk- en Informatiesystemen (Wbni — Dutch NIS Implementation Act)

#### 5.4.1 Basic Information
- **Full Name**: Wet Beveiliging Netwerk- en Informatiesystemen (Act on Security of Network and Information Systems)
- **Reference**: Wbni (2018, implementing NIS Directive 2016/1148; will be updated for NIS2)
- **Purpose**: Transpose NIS Directive into Dutch law (to be replaced by NIS2 transposition)
- **Enforcement**: Sector-specific authorities (DNB for banking sector)

#### 5.4.2 Scope
- Banks as operators of essential services
- Cybersecurity requirements for critical IT systems

#### 5.4.3 Key Obligations
- Cybersecurity risk management measures
- Incident reporting to DNB
- Compliance with sector-specific guidelines (DNB Good Practices)

**IS Impact**: Aligned with DNB Guidelines above

#### 5.4.4 Compliance Status
- **Status**: Compliant
- **NIS2 Monitoring**: Legal team tracking Dutch transposition of NIS2 Directive
- **Responsible**: CISO, Country Manager (Netherlands)

---

### 5.5 Netherlands Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| UAVG | Dutch GDPR Implementation | Data protection, DPO | DPO | Annually |
| DNB Guidelines | Various publications | IT governance, operational resilience, third-party risk | Country Mgr (NL), CISO | Annually |
| Wbni (NIS) | NIS Implementation Act | Cybersecurity, incident reporting | CISO | Annually (pending NIS2 update) |

---

## 6. Spain

### 6.1 Overview
Spain has comprehensive data protection legislation (LOPDGDD) supplementing GDPR, and the Banco de España issues circulars on IT and operational risk management for banks.

---

### 6.2 LOPDGDD (Ley Orgánica de Protección de Datos Personales y Garantía de los Derechos Digitales)

#### 6.2.1 Basic Information
- **Full Name**: Ley Orgánica 3/2018 de Protección de Datos Personales y garantía de los derechos digitales (Organic Law on Personal Data Protection and Guarantee of Digital Rights)
- **Reference**: LOPDGDD (Organic Law 3/2018)
- **Effective Date**: 7 December 2018
- **Purpose**: Spanish implementation and supplementation of GDPR
- **Enforcement**: AEPD (Agencia Española de Protección de Datos — Spanish Data Protection Authority)

#### 6.2.2 Scope
- All processing of personal data by EuroTrust Bank AG in Spain
- Includes Madrid branch and Spanish customers

#### 6.2.3 Key Information Security Obligations

##### Title II: Principles of Data Protection
- Supplements GDPR principles with Spanish-specific interpretations
- Employee data processing (employment context)

**IS Impact**: Data protection policies aligned with Spanish law, HR systems

##### Title IV: DPO
- DPO appointment required (consistent with GDPR)
- DPO must be registered with AEPD

**IS Impact**: DPO function covers Spain, AEPD registration

##### Title X: Digital Rights Guarantee
- Rights related to digital disconnection (employee rights)
- Digital privacy in the workplace
- Limitation of employee surveillance

**IS Impact**: Employee monitoring policies, limitations on workplace surveillance, access logging policies

##### Article 94: Security of Processing Systems
- Duty to implement appropriate security measures
- Alignment with GDPR Article 32

**IS Impact**: Security controls for Spanish operations

#### 6.2.4 Compliance Status
- **Status**: Compliant
- **AEPD Registration**: Completed
- **Responsible**: DPO, Country Manager (Spain)

---

### 6.3 Banco de España Circulars on IT Risk

#### 6.3.1 Basic Information
- **Full Name**: Various circulars and guidelines issued by Banco de España
- **Key Circular**: Circular 2/2016 on Supervision and Solvency (includes IT and operational risk)
- **Purpose**: Supervisory expectations for banks operating in Spain
- **Enforcement**: Banco de España (supervisory reviews)

#### 6.3.2 Scope
- IT governance and risk management
- Operational continuity
- Outsourcing

#### 6.3.3 Key Information Security Obligations

##### IT Governance
- Clear responsibilities for IT management
- IT strategy approved by senior management
- Alignment with EBA Guidelines

**IS Impact**: IT governance for Spanish operations

##### Operational Continuity
- Business continuity plans for Spanish branches
- Identification of critical functions
- Testing requirements

**IS Impact**: Spain-specific BCP, coordination with enterprise BCP

##### Outsourcing
- Notification to Banco de España for material outsourcing
- Contractual requirements
- Right to access and audit

**IS Impact**: Outsourcing notifications to Banco de España (e.g., AWS usage)

#### 6.3.4 Compliance Status
- **Status**: Compliant
- **Last Banco de España Review**: 2025
- **Responsible**: Country Manager (Spain), CISO

---

### 6.4 Spain Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| LOPDGDD | Organic Law 3/2018 | Data protection, digital rights, employee monitoring | DPO | Annually |
| Banco de España Circulars | Circular 2/2016 (and others) | IT governance, BCP, outsourcing | Country Mgr (ES), CISO | Annually |

---

## 7. Poland

### 7.1 Overview
Poland has enacted a comprehensive National Cybersecurity System Act, transposing the NIS Directive and establishing detailed cybersecurity obligations. KNF (Polish Financial Supervision Authority) provides additional guidance for banks.

---

### 7.2 Polish Personal Data Protection Act (Implementing GDPR)

#### 7.2.1 Basic Information
- **Full Name**: Ustawa z dnia 10 maja 2018 r. o ochronie danych osobowych (Act of 10 May 2018 on Personal Data Protection)
- **Reference**: Polish Data Protection Act (2018)
- **Effective Date**: 25 May 2018
- **Purpose**: Polish implementation of GDPR
- **Enforcement**: UODO (Urząd Ochrony Danych Osobowych — Polish Data Protection Authority)

#### 7.2.2 Scope
- All processing of personal data by EuroTrust Bank AG in Poland (Warsaw branch)

#### 7.2.3 Key Information Security Obligations

##### DPO Requirements
- DPO mandatory for financial institutions
- Registration with UODO

**IS Impact**: DPO function covers Poland, UODO registration

##### Security Measures
- Aligned with GDPR Article 32
- Implementation of appropriate technical and organizational measures

**IS Impact**: Security controls for Polish operations

#### 7.2.4 Compliance Status
- **Status**: Compliant
- **UODO Registration**: Completed
- **Responsible**: DPO, Country Manager (Poland)

---

### 7.3 Act on the National Cybersecurity System

#### 7.3.1 Basic Information
- **Full Name**: Ustawa z dnia 5 lipca 2018 r. o krajowym systemie cyberbezpieczeństwa (Act on the National Cybersecurity System)
- **Reference**: Polish Cybersecurity Act (2018, as amended)
- **Effective Date**: 28 August 2018
- **Purpose**: Implement NIS Directive, establish national cybersecurity framework
- **Enforcement**: CSIRT NASK (National CSIRT), sector-specific authorities (KNF for banking)

#### 7.3.2 Scope
- Banks classified as **operators of essential services**
- IT systems supporting critical banking functions

#### 7.3.3 Key Information Security Obligations

##### Article 8: Cybersecurity Risk Management
- Implement risk management systems for network and information systems
- Measures to prevent, detect, respond to, and recover from incidents
- Regular risk assessments

**IS Impact**: Cybersecurity risk management framework for Poland, risk assessments

##### Article 11: Security Measures
- Implement appropriate organizational and technical measures:
  - Security policies
  - Incident handling procedures
  - Business continuity
  - Access control
  - Protection of information systems
  - Cryptography
  - Logging and monitoring

**IS Impact**: Comprehensive security controls for Polish operations

##### Article 13: Incident Reporting
- Report significant cybersecurity incidents to CSIRT NASK and KNF
- **Timeframes**:
  - Initial notification: Without undue delay
  - Detailed report: Within 72 hours
  - Final report: Within 1 month

**IS Impact**: Incident reporting procedures to Polish authorities (CSIRT NASK, KNF)

##### Article 17: Cybersecurity Audits
- Periodic audits of cybersecurity measures (frequency based on risk assessment, typically every 2 years)
- Conducted by certified auditors

**IS Impact**: Cybersecurity audit program for Poland, engagement of certified auditors

#### 7.3.4 Compliance Status
- **Status**: Compliant
- **Last Cybersecurity Audit (Poland)**: 2024
- **Next Audit**: 2026
- **Responsible**: CISO, Country Manager (Poland)

---

### 7.4 KNF Guidelines on IT and Security Risk Management

#### 7.4.1 Basic Information
- **Full Name**: KNF (Komisja Nadzoru Finansowego) Recommendations and Guidelines on IT Risk Management
- **Key Document**: KNF Recommendation D on risk management systems in banks (includes IT risk)
- **Purpose**: Supervisory expectations for banks' IT and security risk management
- **Enforcement**: KNF (supervisory reviews, inspections)

#### 7.4.2 Scope
- IT risk management
- Information security
- Operational resilience

#### 7.4.3 Key Information Security Obligations

##### IT Risk Management
- IT risk management process integrated into overall risk management
- IT risk appetite and limits
- Regular IT risk assessments

**IS Impact**: IT risk management framework for Poland

##### Information Security
- Information security policies and procedures
- Access control and identity management
- Cryptographic controls
- Incident management

**IS Impact**: Information security policies for Poland, aligned with enterprise ISMS

##### Business Continuity
- BCP and DR plans for Polish operations
- Testing requirements

**IS Impact**: Poland-specific BCP, coordination with enterprise BCP

#### 7.4.4 Compliance Status
- **Status**: Compliant
- **Last KNF Review**: 2024
- **Responsible**: Country Manager (Poland), CISO

---

### 7.5 Poland Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| Polish Data Protection Act | Act of 10 May 2018 | Data protection, DPO | DPO | Annually |
| National Cybersecurity System Act | Act of 5 July 2018 | Cybersecurity risk mgmt, incident reporting, audits | CISO | Annually |
| KNF Recommendations | Recommendation D | IT risk management, information security, BCP | Country Mgr (PL), CISO | Annually |

---

## 8. Ireland

### 8.1 Overview
Ireland serves as an important EU hub for EuroTrust Bank AG, hosting regulatory and treasury operations. The Data Protection Commission (DPC) is a leading European data protection authority, and the Central Bank of Ireland (CBI) has comprehensive IT and cyber resilience expectations.

---

### 8.2 Data Protection Act 2018

#### 8.2.1 Basic Information
- **Full Name**: Data Protection Act 2018
- **Reference**: Act No. 7 of 2018
- **Effective Date**: 24 May 2018 (immediately before GDPR application)
- **Purpose**: Irish implementation and supplementation of GDPR
- **Enforcement**: DPC (Data Protection Commission — Ireland's lead supervisory authority)

#### 8.2.2 Scope
- All processing of personal data by EuroTrust Bank AG in Ireland (Dublin office)
- Ireland is a key location for data protection compliance given DPC's prominence

#### 8.2.3 Key Information Security Obligations

##### Part 2: GDPR Provisions
- Supplements GDPR with Irish-specific provisions
- Age of consent (16 years for children's data)
- Specific provisions for processing employment data

**IS Impact**: Data protection policies for Ireland, HR systems

##### Part 5: DPO
- DPO appointment and independence
- Registration with DPC

**IS Impact**: DPO function covers Ireland, DPC engagement

##### Section 96: Security of Processing
- Reinforces GDPR Article 32 obligations
- Appropriate security measures based on risk

**IS Impact**: Security controls for Irish operations

#### 8.2.4 Compliance Status
- **Status**: Compliant
- **DPC Registration**: Completed
- **Responsible**: DPO, Country Manager (Ireland)

---

### 8.3 Central Bank of Ireland — Cross Industry Guidance on Information Technology and Cybersecurity Risks

#### 8.3.1 Basic Information
- **Full Name**: Cross Industry Guidance: Information Technology and Cybersecurity Risks
- **Issuer**: Central Bank of Ireland (CBI)
- **Publication Date**: November 2016 (updated with Dear CEO letter in 2023)
- **Purpose**: Supervisory expectations for financial institutions' IT and cybersecurity practices
- **Enforcement**: CBI (supervisory reviews, themed inspections)

#### 8.3.2 Scope
- IT governance and strategy
- Cybersecurity risk management
- Operational resilience
- Third-party risk

#### 8.3.3 Key Information Security Obligations

##### Governance and Oversight
- Board-level oversight of IT and cybersecurity risks
- IT strategy aligned with business objectives
- Regular reporting to the Board on IT and cyber risks

**IS Impact**: IT governance for Ireland, Board reporting requirements

##### Cybersecurity Risk Management
- Comprehensive cybersecurity framework
- Risk assessments of IT systems
- Security controls aligned with recognized standards (ISO 27001, NIST Cybersecurity Framework)

**IS Impact**: Cybersecurity risk management for Ireland, alignment with ISO 27001 ISMS

##### Operational Resilience
- Business continuity and disaster recovery capabilities
- Regular testing of resilience (including cyber incident scenarios)
- Recovery objectives (RTO/RPO)

**IS Impact**: Ireland-specific BCP, coordination with enterprise BCP

##### Third-Party Risk Management
- Due diligence on critical IT service providers
- Contractual arrangements with security clauses
- Ongoing monitoring and audit rights
- Concentration risk management (e.g., cloud providers)

**IS Impact**: Vendor risk assessments for Ireland-based services, cloud governance

##### Incident Management
- Cyber incident response plan
- Incident reporting to CBI for significant incidents
- Post-incident review and lessons learned

**IS Impact**: Incident response procedures for Ireland, CBI reporting

##### Threat Intelligence and Security Monitoring
- Continuous monitoring of security threats
- Participation in information-sharing initiatives
- Security Operations Centre (SOC) capabilities

**IS Impact**: Threat intelligence integration, SOC monitoring for Ireland operations

#### 8.3.4 CBI Dear CEO Letters
- CBI issues periodic "Dear CEO" letters highlighting supervisory priorities
- Recent focus areas: cyber resilience, operational resilience, third-party risk, cloud adoption

**IS Impact**: Ongoing monitoring of CBI supervisory expectations, management responses

#### 8.3.5 Compliance Status
- **Status**: Compliant
- **Last CBI Review**: 2025
- **Responsible**: Country Manager (Ireland), CISO

---

### 8.4 Ireland Summary

| Regulation | Reference | Key IS Obligations | Responsible Owner | Review Frequency |
|------------|-----------|-------------------|-------------------|------------------|
| Data Protection Act 2018 | Act No. 7 of 2018 | Data protection, DPO, security measures | DPO | Annually |
| CBI Cross Industry Guidance | CBI Guidance (2016/2023) | IT governance, cybersecurity, operational resilience, third-party risk | Country Mgr (IE), CISO | Annually |

---

## 9. Cross-Country Coordination

### 9.1 Challenges
- **Divergent National Requirements**: Despite harmonization efforts (GDPR, DORA, NIS2), national variations persist
- **Multiple Supervisors**: Six national banking supervisors, six data protection authorities, multiple cybersecurity authorities
- **Incident Reporting**: Overlapping incident notification obligations to national authorities
- **Language Requirements**: Certain regulatory communications must be in national languages

### 9.2 EuroTrust Bank AG Coordination Mechanisms

#### 9.2.1 Governance
- **Group Compliance Committee**: Quarterly meetings with country compliance representatives
- **Information Security Council**: Monthly meetings including country CISOs/InfoSec leads
- **Data Protection Forum**: Bi-monthly meetings coordinated by Group DPO

#### 9.2.2 Policies and Procedures
- **Group Policies**: Centrally developed, locally adapted where required by national law
- **Local Procedures**: Country-specific procedures for regulatory reporting, incident notification
- **Language Support**: Key policies translated into German, French, Dutch, Spanish, Polish

#### 9.2.3 Regulatory Reporting
- **Centralized Incident Tracking**: Incidents logged in central system with regulatory reporting requirements mapped
- **Country Notification Matrix**: Matrix mapping incident types to national notification obligations
- **Coordination Protocol**: Process for notifying multiple authorities in case of cross-border incidents

#### 9.2.4 Training and Awareness
- **Group Training**: Annual information security and compliance training (mandatory for all employees)
- **Country-Specific Modules**: Additional training on national requirements (e.g., BAIT for Germany, LPM for France)

---

## 10. Summary of Compliance Responsibilities

| Country | Regulations | Primary Country Owner | Group Support | Review Frequency |
|---------|-------------|----------------------|---------------|------------------|
| Germany | BDSG, KWG, BAIT, IT-SiG 2.0 | Country Manager (DE) | DPO, CISO, CRO | Semi-annually |
| France | Loi Informatique et Libertés, ACPR Guidelines, LPM | Country Manager (FR) | DPO, CISO | Annually |
| Netherlands | UAVG, DNB Guidelines, Wbni | Country Manager (NL) | DPO, CISO | Annually |
| Spain | LOPDGDD, Banco de España Circulars | Country Manager (ES) | DPO, CISO | Annually |
| Poland | Data Protection Act, Cybersecurity Act, KNF Guidelines | Country Manager (PL) | DPO, CISO | Annually |
| Ireland | Data Protection Act 2018, CBI Guidance | Country Manager (IE) | DPO, CISO | Annually |

---

## 11. Regulatory Horizon Scanning (National Level)

### 11.1 Germany
- **NIS2 Transposition**: Expected by October 2024 (monitoring implementation into BSIG)
- **DORA Implementation**: BaFin guidance on DORA compliance (forthcoming)

### 11.2 France
- **LPM 2024-2030**: Updated Military Programming Law (potential changes to OIV regime)
- **ANSSI Certification**: Evolving requirements for security product qualifications

### 11.3 Netherlands
- **NIS2 Transposition**: Update to Wbni expected 2024-2025
- **DNB Thematic Reviews**: Ongoing focus on cyber resilience and third-party risk

### 11.4 Spain
- **NIS2 Transposition**: Spanish implementation expected 2024-2025
- **Cybersecurity Certification Schemes**: Potential national adoption of EU cybersecurity certification

### 11.5 Poland
- **Cybersecurity Act Amendments**: Potential updates to align with NIS2
- **KNF Focus Areas**: Increased scrutiny on cloud outsourcing

### 11.6 Ireland
- **NIS2 Transposition**: Irish legislation expected 2024-2025
- **CBI Operational Resilience**: Enhanced expectations following UK precedent

---

## 12. Document Maintenance

### 12.1 Review Schedule
- **Frequency**: Quarterly
- **Next Scheduled Review**: April 2026
- **Owner**: Chief Compliance Officer, supported by Legal Counsel

### 12.2 Change Process
- National legal developments → Country Manager notifies Group Compliance → Legal analysis → Impact assessment → Policy updates → Executive approval

---

## Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Legal & Compliance Teams | Initial version for ISO 27001 audit |

---

**END OF DOCUMENT**

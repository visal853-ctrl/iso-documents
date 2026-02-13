# Contractual Requirements — Legal & Regulatory Requirements

## Document Control
- **Document ID**: LRR-CR-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal - Confidential
- **Owner**: Chief Compliance Officer (CCO) & Chief Legal Officer

---

## 1. Introduction

This document identifies and catalogues **contractual obligations** related to information security arising from EuroTrust Bank AG's agreements with third-party service providers, industry standards bodies, payment networks, and customers. These contractual requirements are legally binding and form part of the organization's compliance obligations under **ISO/IEC 27002:2022 Control 5.31**.

Contractual requirements complement legal and regulatory obligations and must be managed with equal rigor to avoid breach of contract, service disruptions, regulatory penalties, and reputational damage.

---

## 2. Contractual Requirements Summary

| # | Contract Category | Counterparty/Source | Key IS Obligations | Owner |
|---|-------------------|---------------------|-------------------|-------|
| 1 | Cloud Service Provider | Amazon Web Services (AWS) | Data processing, security controls, audit rights, data residency | CIO/CISO |
| 2 | Payment Card Industry | PCI Security Standards Council | PCI DSS compliance, cardholder data protection | Head of Payments |
| 3 | International Payments | SWIFT (Society for Worldwide Interbank Financial Telecommunication) | SWIFT CSP requirements, cybersecurity controls | Head of Treasury |
| 4 | Correspondent Banking | Multiple correspondent banks | Information security clauses, incident notification | Head of Treasury |
| 5 | Outsourcing Agreements | Various vendors (IT, operations) | EBA Outsourcing Guidelines, security obligations, audit rights | Procurement/CISO |
| 6 | Customer Contracts | Retail & corporate customers | Data protection, privacy clauses, security commitments | Legal/CCO |
| 7 | Confidentiality Agreements | Third parties (vendors, partners) | NDAs, confidentiality obligations, data handling | Legal |
| 8 | Cyber Insurance | Insurance provider | Security controls, incident reporting, breach notification | CRO |
| 9 | Interbank Networks | SEPA, TARGET2, EBA Clearing | Operational security, availability, incident response | Head of Treasury |
| 10 | Software Licensing | Microsoft, CrowdStrike, Splunk, etc. | Licensing compliance, security configurations | CIO/IT |

---

## 3. Detailed Contractual Requirements

### 3.1 Cloud Service Provider — Amazon Web Services (AWS)

#### 3.1.1 Contract Information
- **Counterparty**: Amazon Web Services EMEA SARL (Luxembourg)
- **Contract Type**: AWS Customer Agreement + AWS Business Associate Agreement (BAA) + Standard Contractual Clauses (SCCs)
- **Effective Date**: January 2023
- **Term**: Ongoing (monthly billing)
- **AWS Regions Used**: eu-central-1 (Frankfurt), eu-west-1 (Ireland), eu-west-3 (Paris)
- **Services**: Compute (EC2), storage (S3), databases (RDS, Aurora), serverless (Lambda), security (GuardDuty, Security Hub), backup (AWS Backup)

#### 3.1.2 Key Information Security Obligations

##### 3.1.2.1 Data Processing Agreement (DPA) / Standard Contractual Clauses
- **Obligation**: AWS acts as a **data processor** under GDPR; EuroTrust Bank AG is the **data controller**
- **SCCs**: EU Standard Contractual Clauses for data transfers (Module 2: Controller to Processor)
- **Data Residency**: Personal data of EU customers must remain in EU AWS regions
- **Sub-processors**: AWS maintains list of sub-processors; notification of changes with right to object

**IS Impact**:
- Data localization controls in AWS (restrict services to EU regions)
- Configuration of AWS Organizations to enforce geographic restrictions
- Sub-processor review and approval process

##### 3.1.2.2 AWS Shared Responsibility Model
- **AWS Responsibility**: Security **of** the cloud (physical infrastructure, network, hypervisor)
- **Customer Responsibility** (EuroTrust Bank AG): Security **in** the cloud (data, applications, IAM, encryption, network configuration)

**IS Impact**:
- Implementation of customer-side security controls:
  - Encryption at rest (AWS KMS for encryption keys)
  - Encryption in transit (TLS 1.3)
  - Identity and Access Management (IAM policies, MFA for AWS Console)
  - Security groups and network ACLs
  - Logging and monitoring (CloudTrail, CloudWatch, GuardDuty)
  - Vulnerability management for customer-managed EC2 instances

##### 3.1.2.3 Compliance Certifications
- **AWS Commitments**: AWS maintains certifications including ISO 27001, SOC 2 Type II, PCI DSS Level 1, C5 (Germany)
- **Audit Reports**: EuroTrust Bank AG has right to request AWS compliance reports (SOC 2, ISO 27001 certificates)

**IS Impact**:
- Annual review of AWS compliance reports
- Evidence collection for ISO 27001 audit (AWS as critical third party)

##### 3.1.2.4 Security Incident Notification
- **AWS Obligation**: Notify EuroTrust Bank AG of security incidents affecting customer data or services
- **Timeframe**: Without undue delay
- **Channel**: AWS Support, AWS Security bulletins

**IS Impact**:
- Monitoring of AWS security bulletins and Health Dashboard
- Integration of AWS incident notifications into EuroTrust incident response process
- Potential regulatory reporting obligations triggered by AWS incidents (GDPR, DORA, NIS2)

##### 3.1.2.5 Right to Audit
- **Contractual Provision**: EuroTrust Bank AG has right to audit AWS, subject to AWS standard audit process
- **Practical Implementation**: AWS provides third-party audit reports (SOC 2, ISO 27001) in lieu of individual audits

**IS Impact**:
- Annual review of AWS audit reports as evidence of security controls
- Documentation for regulatory inspections (BaFin, ECB, national authorities)

##### 3.1.2.6 Data Deletion
- **Obligation**: Upon termination, AWS deletes customer data in accordance with AWS data retention policies
- **Timeframe**: Customer data deleted within 90 days of account closure

**IS Impact**:
- Exit planning for AWS migration or termination
- Data extraction procedures before account closure

##### 3.1.2.7 Service Level Agreements (SLAs)
- **Availability Commitments**: AWS provides SLAs for individual services (e.g., EC2: 99.99% uptime for multi-AZ deployments)
- **Service Credits**: Financial credits if SLA not met

**IS Impact**:
- Architectural design for high availability (multi-AZ deployments)
- Monitoring of AWS service availability (CloudWatch, AWS Health)
- Integration with business continuity and disaster recovery planning

#### 3.1.3 Compliance Status
- **Status**: Compliant
- **Last Contract Review**: January 2026
- **Last AWS Audit Report Review**: December 2025 (SOC 2 Type II for FY2025)
- **Next Review**: July 2026

#### 3.1.4 Responsible Department/Role
- **Primary Owner**: Chief Information Officer (CIO)
- **Supporting**: CISO, Compliance, Legal, Cloud Governance Team
- **AWS Account Management**: Cloud Platform Team

---

### 3.2 Payment Card Industry Data Security Standard (PCI DSS)

#### 3.2.1 Contract Information
- **Standard Body**: PCI Security Standards Council
- **Standard**: PCI DSS v4.0 (Payment Card Industry Data Security Standard, version 4.0)
- **Applicability**: Mandatory compliance for processing Mastercard and Visa card payments
- **Merchant Level**: Level 1 Merchant (>6 million transactions annually)
- **Service Provider Level**: Level 1 Service Provider (if providing payment services to other entities)
- **Acquirer**: EuroTrust Bank AG uses third-party acquirers (contractual flow-down of PCI DSS requirements)

#### 3.2.2 Key Information Security Obligations

##### 3.2.2.1 Cardholder Data Environment (CDE)
- **Requirement**: Define and secure the **Cardholder Data Environment** (CDE)
- **CDE Scope**: Systems that store, process, or transmit cardholder data (CHD) or sensitive authentication data (SAD)

**IS Impact**:
- Segmentation of card payment systems from other networks
- Network diagram of CDE
- Firewall rules restricting access to CDE

##### 3.2.2.2 PCI DSS Requirements (12 Requirements, 300+ Sub-Requirements)

**Requirement 1: Install and Maintain Network Security Controls**
- Firewalls and network segmentation to protect CDE

**Requirement 2: Apply Secure Configurations to All System Components**
- Hardening of servers, network devices, payment terminals
- Change default passwords and security parameters

**Requirement 3: Protect Stored Account Data**
- Encryption of cardholder data at rest (AES-256)
- Minimize data retention (delete data when no longer needed)
- **Prohibition**: Never store sensitive authentication data after authorization (CVV2, full magnetic stripe, PIN)

**Requirement 4: Protect Cardholder Data with Strong Cryptography During Transmission**
- TLS 1.2+ for cardholder data transmission
- End-to-end encryption for payment transactions

**Requirement 5: Protect All Systems and Networks from Malicious Software**
- Anti-malware on all systems in CDE
- Regular updates and scans

**Requirement 6: Develop and Maintain Secure Systems and Software**
- Secure software development lifecycle (SDLC)
- Patch management (critical patches within 30 days)
- Vulnerability scans and penetration testing

**Requirement 7: Restrict Access to System Components and Cardholder Data by Business Need to Know**
- Role-based access control (RBAC)
- Least privilege principle

**Requirement 8: Identify Users and Authenticate Access to System Components**
- Unique user IDs for all personnel
- Multi-factor authentication (MFA) for access to CDE

**Requirement 9: Restrict Physical Access to Cardholder Data**
- Physical security controls for data centres and offices housing CDE components
- Visitor logs, badge access

**Requirement 10: Log and Monitor All Access to System Components and Cardholder Data**
- Centralized logging (SIEM integration)
- Log retention (minimum 1 year, 3 months online)
- Daily log review

**Requirement 11: Test Security of Systems and Networks Regularly**
- **Quarterly external vulnerability scans** by PCI Approved Scanning Vendor (ASV)
- **Annual penetration testing** (network and application layers)
- Intrusion detection/prevention systems (IDS/IPS)

**Requirement 12: Support Information Security with Organizational Policies and Programs**
- PCI DSS security policy
- Annual security awareness training
- Incident response plan specific to payment card incidents

**IS Impact**:
- Comprehensive security program for CDE aligned with PCI DSS
- Dedicated resources for PCI DSS compliance
- Annual on-site assessment (Report on Compliance — ROC)

##### 3.2.2.3 Annual Compliance Validation
- **Requirement**: Annual PCI DSS assessment by Qualified Security Assessor (QSA)
- **Deliverables**: Report on Compliance (ROC), Attestation of Compliance (AOC)
- **Submission**: AOC submitted to payment brands (Mastercard, Visa) and acquirers

**IS Impact**:
- Annual QSA engagement (typically Q3 each year)
- Remediation of findings before AOC issuance
- Quarterly Self-Assessment Questionnaires (SAQs) for service providers

##### 3.2.2.4 Quarterly Vulnerability Scans
- **Requirement**: Quarterly external vulnerability scans by PCI Approved Scanning Vendor (ASV)
- **Scope**: All external-facing IP addresses in CDE scope
- **Passing Score**: No vulnerabilities rated 4.0 or higher (CVSS scale)

**IS Impact**:
- Engagement with ASV (e.g., Qualys, Trustwave)
- Quarterly scan schedule (Q1, Q2, Q3, Q4)
- Remediation of vulnerabilities before rescan

##### 3.2.2.5 Data Breach Notification
- **Obligation**: Notify payment brands and acquirers immediately upon discovery of a breach involving cardholder data
- **Forensic Investigation**: Engage PCI Forensic Investigator (PFI) for breach investigation
- **Fines and Penalties**: Payment brands may impose fines for breaches and non-compliance

**IS Impact**:
- Payment card breach response plan
- Relationship with PCI Forensic Investigator (pre-arranged)
- Financial provisioning for potential fines

#### 3.2.3 Compliance Status
- **Status**: Compliant (PCI DSS v4.0)
- **Last QSA Assessment**: September 2025
- **AOC Valid Until**: September 2026
- **Last ASV Scan**: January 2026 (Passed)
- **Next ASV Scan**: April 2026

#### 3.2.4 Responsible Department/Role
- **Primary Owner**: Head of Payments & Digital Banking
- **Supporting**: CISO, IT Security, Compliance
- **QSA Relationship**: Managed by Compliance Officer
- **PCI DSS Compliance Manager**: Dedicated role within IT Security team

---

### 3.3 SWIFT Customer Security Programme (CSP)

#### 3.3.1 Contract Information
- **Counterparty**: SWIFT SCRL (Society for Worldwide Interbank Financial Telecommunication)
- **Programme**: SWIFT Customer Security Programme (CSP)
- **Effective Date**: January 2018 (mandatory for all SWIFT users)
- **Applicability**: All SWIFT-connected systems and users at EuroTrust Bank AG
- **CSP Version**: CSP 2025 (annual updates)

#### 3.3.2 Key Information Security Obligations

##### 3.3.2.1 SWIFT Customer Security Controls Framework (CSCF)
- **Mandatory Controls**: 21 mandatory security controls (as of CSP 2025)
- **Advisory Controls**: Additional recommended controls
- **Self-Attestation**: Annual attestation of compliance with mandatory controls

**Mandatory Control Categories**:
1. **Secure Your Environment** (Controls 1.1 - 1.5)
   - Restrict internet access from SWIFT environment
   - Physical and logical security of SWIFT infrastructure
   - Segregation of SWIFT environment from general IT

2. **Know and Limit Access** (Controls 2.1 - 2.8)
   - User access management for SWIFT systems
   - Multi-factor authentication (MFA)
   - Privileged access management
   - User activity monitoring

3. **Reduce Attack Surface** (Controls 3.1 - 3.3)
   - Operating system patching
   - Application patching
   - Database patching

4. **Detect Anomalous Activity** (Controls 4.1 - 4.2)
   - Transaction monitoring and reconciliation
   - Security monitoring and detection

5. **Plan for Incident Response and Information Sharing** (Controls 5.1 - 5.3)
   - Incident response planning
   - Information sharing with SWIFT and community
   - Cybersecurity training and awareness

**IS Impact**:
- Dedicated SWIFT security controls program
- Network segmentation (SWIFT zone isolated from general IT network)
- Enhanced monitoring of SWIFT environment
- Annual gap analysis and remediation plan

##### 3.3.2.2 Annual Attestation
- **Requirement**: Annual self-attestation of compliance with SWIFT CSP mandatory controls
- **Deadline**: By year-end (December 31 each year)
- **Evidence**: Supporting documentation and screenshots
- **Independent Assessment**: Optional but recommended — external assessor validates attestation

**IS Impact**:
- Annual CSP assessment process (typically Q3-Q4)
- Collection of evidence (configurations, policies, access reviews)
- Submission of attestation via SWIFT Customer Security Controls (CSC) questionnaire

##### 3.3.2.3 KYC Security Attestation
- **Requirement**: Share security attestation with correspondent banks and counterparties as part of KYC (Know Your Customer) process
- **Purpose**: Enable counterparties to assess EuroTrust Bank AG's SWIFT security posture

**IS Impact**:
- Distribution of SWIFT CSP attestation to correspondent banks
- Response to counterparty security questionnaires
- Documentation for KYC due diligence

##### 3.3.2.4 Incident Reporting to SWIFT
- **Obligation**: Report cyber incidents affecting SWIFT infrastructure or messaging to SWIFT
- **Timeframe**: As soon as reasonably possible
- **Channel**: SWIFT Customer Security Incident Reporting (CSIR) portal

**IS Impact**:
- Integration of SWIFT incident reporting into incident response procedures
- Classification criteria for SWIFT-reportable incidents
- Coordination with SWIFT CSIRT (Computer Security Incident Response Team)

##### 3.3.2.5 Mandatory Software Updates
- **SWIFT Alliance Access Updates**: Security patches and software updates must be applied in accordance with SWIFT release schedules
- **Vulnerability Management**: Critical vulnerabilities in SWIFT software must be remediated promptly

**IS Impact**:
- Patch management schedule for SWIFT systems
- Testing of SWIFT software updates before production deployment
- Coordination with SWIFT support for maintenance windows

##### 3.3.2.6 Segregation of SWIFT Environment
- **Control 1.1**: Internet connectivity from SWIFT environment must be restricted
- **Best Practice**: Physical or logical segregation of SWIFT infrastructure (dedicated servers, network zone)

**IS Impact**:
- Network architecture: SWIFT zone with firewall isolation
- Jump servers for administrator access to SWIFT environment
- Prohibition of direct internet access from SWIFT systems

#### 3.3.3 Compliance Status
- **Status**: Compliant (SWIFT CSP 2025)
- **Last Attestation**: December 2025
- **Independent Assessment**: Completed by external assessor (November 2025)
- **Next Attestation**: December 2026

#### 3.3.4 Responsible Department/Role
- **Primary Owner**: Head of Treasury & International Payments
- **Supporting**: CISO, IT Security, Network Engineering
- **SWIFT Security Manager**: Dedicated role within Treasury Operations
- **SWIFT Technical Team**: IT infrastructure team managing SWIFT systems

---

### 3.4 Correspondent Banking Agreements

#### 3.4.1 Contract Information
- **Counterparties**: Multiple correspondent banks in various jurisdictions (e.g., JPMorgan Chase, Deutsche Bank, BNP Paribas, HSBC, etc.)
- **Purpose**: Facilitate international payments, nostro account management, foreign exchange settlement
- **Contract Type**: Master Correspondent Banking Agreement (MCBA), bilateral agreements
- **Number of Correspondents**: ~50 global correspondent banks

#### 3.4.2 Key Information Security Obligations

##### 3.4.2.1 Information Security Clauses
- **Standard Clause**: Correspondents require EuroTrust Bank AG to maintain appropriate information security controls
- **SWIFT CSP Compliance**: Many correspondents require evidence of SWIFT CSP compliance (see Section 3.3)
- **Cybersecurity Questionnaires**: Periodic cybersecurity due diligence questionnaires from correspondents

**IS Impact**:
- Response to correspondent security questionnaires (coordinated by Compliance and CISO)
- Sharing of SWIFT CSP attestation and other security certifications (ISO 27001, SOC 2)

##### 3.4.2.2 Incident Notification
- **Obligation**: Notify correspondent banks of cybersecurity incidents that may affect payment processing or correspondent relationship
- **Examples**: Ransomware affecting payment systems, SWIFT environment compromise, data breach involving correspondent transactions

**IS Impact**:
- Incident notification procedures for correspondent banks
- Communication templates for incident disclosure
- Legal review of notification obligations in each correspondent agreement

##### 3.4.2.3 Audit Rights
- **Provision**: Some correspondent agreements grant mutual audit rights
- **Practical Implementation**: Typically satisfied through sharing of third-party audit reports (SOC 2, ISO 27001)

**IS Impact**:
- Maintenance of audit reports for sharing with correspondents
- Hosting of correspondent auditors for on-site reviews (rare)

##### 3.4.2.4 Data Protection and Confidentiality
- **Obligation**: Protect confidentiality of transaction data, account information, and correspondent communications
- **GDPR Considerations**: Cross-border data transfers to non-EEA correspondents (adequacy decisions, SCCs, or derogations)

**IS Impact**:
- Encryption of correspondent communications (SWIFT messages, secure email)
- Access controls for correspondent transaction data
- Data protection impact assessments (DPIAs) for transfers to non-EEA correspondents

##### 3.4.2.5 Sanctions and AML Compliance
- **Indirect IS Impact**: Correspondent agreements require compliance with sanctions screening and AML/CFT
- **Technology**: Transaction monitoring systems must securely process and screen correspondent transactions

**IS Impact**:
- Security of AML/sanctions screening systems
- Audit trails for sanctions screening
- Data retention for correspondent transactions (5 years minimum)

#### 3.4.3 Compliance Status
- **Status**: Compliant
- **Correspondent Reviews**: Ongoing (rolling cycle)
- **Last Major Questionnaire Campaign**: Q4 2025 (annual SWIFT CSP sharing)

#### 3.4.4 Responsible Department/Role
- **Primary Owner**: Head of Treasury & Correspondent Banking
- **Supporting**: Compliance, CISO, Legal
- **Questionnaire Coordination**: Compliance Officer (with inputs from CISO for technical questions)

---

### 3.5 Outsourcing Agreements (Governed by EBA Outsourcing Guidelines)

#### 3.5.1 Overview
- **Regulatory Framework**: EBA Guidelines on Outsourcing Arrangements (EBA/GL/2019/02)
- **Applicability**: All outsourcing of material functions or critical or important functions (CIFs)
- **Scope**: IT outsourcing (cloud, managed services), business process outsourcing (BPO), facilities management

#### 3.5.2 Key Categories of Outsourcing

##### 3.5.2.1 Cloud Services (AWS — see Section 3.1)
- Primary example of material outsourcing

##### 3.5.2.2 Managed Security Services
- **Examples**: SIEM managed service (Splunk), endpoint protection (CrowdStrike), vulnerability scanning (Qualys)
- **Security Obligations**: 
  - Service provider security certifications (SOC 2, ISO 27001)
  - Data handling and confidentiality
  - Incident notification
  - Audit rights

##### 3.5.2.3 ATM Network Management
- **Vendor**: External ATM service provider
- **Services**: ATM maintenance, cash replenishment, software updates
- **Security Obligations**:
  - Physical security of ATMs
  - Encryption of PIN blocks
  - Incident reporting (skimming, fraud attempts)

##### 3.5.2.4 Customer Call Centre (Tier 1 Support)
- **Vendor**: Outsourced call centre in Poland
- **Services**: Customer service inquiries, password resets, account information
- **Security Obligations**:
  - Access to customer data (need-to-know basis)
  - Authentication procedures for callers
  - Call recording and audit trails
  - Confidentiality and NDA
  - Background checks for call centre staff

##### 3.5.2.5 Back-Office Document Processing
- **Vendor**: Third-party BPO provider
- **Services**: Document scanning, data entry, archival
- **Security Obligations**:
  - Secure document handling
  - Data protection (GDPR compliance)
  - Destruction of physical documents after processing
  - Access controls to customer information

#### 3.5.3 EBA Outsourcing Guidelines — Contractual Requirements

##### 3.5.3.1 Written Outsourcing Agreement
- **Requirement**: All outsourcing must be governed by a written contract

**Mandatory Contractual Clauses** (per EBA Guidelines):
1. **Clear Description of Service**: Scope, service levels, KPIs
2. **Security and Confidentiality**: Information security obligations, confidentiality clauses, data protection
3. **Audit Rights**: Bank's right to audit service provider (and regulators' right to audit)
4. **Subcontracting**: Prior notification and approval of subcontractors
5. **Data and System Ownership**: Bank retains ownership of data and systems
6. **Data Portability**: Ability to retrieve data and transition to another provider
7. **Incident Notification**: Timely notification of security incidents, breaches, service disruptions
8. **Compliance with Laws**: Service provider's obligation to comply with applicable laws and regulations
9. **Termination Rights**: Exit rights, transition assistance, data return/deletion
10. **Business Continuity**: Service provider's BCP/DR obligations
11. **Regulatory Access**: Regulators' right to access service provider premises and records

**IS Impact**:
- Standard outsourcing contract template incorporating EBA requirements
- Legal review of all outsourcing agreements
- Negotiation of security clauses with vendors

##### 3.5.3.2 Due Diligence Before Outsourcing
- **Requirement**: Risk assessment and due diligence on service provider before outsourcing
- **Due Diligence Areas**: Financial stability, reputation, security certifications, technical capabilities, references

**IS Impact**:
- Vendor risk assessment process (questionnaires, certifications review, site visits)
- Security assessment of vendor controls (aligned with ISO 27001, SOC 2)

##### 3.5.3.3 Notification to Regulators
- **Requirement**: Notify national competent authority (BaFin, ACPR, DNB, etc.) of material outsourcing
- **Timeframe**: Before outsourcing commences (or shortly after, depending on jurisdiction)
- **Content**: Description of service, service provider, location, security measures

**IS Impact**:
- Register of outsourcing arrangements
- Notification process to regulators (coordinated by Compliance)

##### 3.5.3.4 Ongoing Monitoring
- **Requirement**: Continuous monitoring of service provider performance and security
- **Mechanisms**: KPI tracking, incident reviews, periodic audits, certification reviews

**IS Impact**:
- Vendor management program
- Quarterly business reviews (QBRs) with critical vendors
- Annual review of vendor audit reports (SOC 2, ISO 27001)

##### 3.5.3.5 Exit Planning
- **Requirement**: Exit strategy and transition plan for termination of outsourcing
- **Documentation**: Exit plan documented before outsourcing commences

**IS Impact**:
- Documented exit plans for each material outsourcing arrangement
- Data extraction procedures
- Transition timelines and resources

#### 3.5.4 Compliance Status
- **Status**: Compliant
- **Outsourcing Register**: Maintained (24 material outsourcing arrangements as of February 2026)
- **Regulator Notifications**: Up to date (all material outsourcing notified)
- **Last Vendor Risk Review**: Q1 2026 (ongoing rolling reviews)

#### 3.5.5 Responsible Department/Role
- **Primary Owner**: Procurement & Vendor Management
- **Supporting**: CISO, Compliance, Legal, CRO
- **Outsourcing Governance**: Third-Party Risk Committee (quarterly meetings)

---

### 3.6 Customer Contracts — Data Protection & Privacy Clauses

#### 3.6.1 Overview
- **Scope**: Terms and conditions, account opening agreements, service agreements with retail and corporate customers
- **Regulatory Basis**: GDPR, national data protection laws, PSD2
- **Purpose**: Establish legal basis for data processing, communicate privacy rights, obtain consent where required

#### 3.6.2 Key Information Security Commitments to Customers

##### 3.6.2.1 Privacy Notices
- **Obligation**: Provide clear and transparent privacy notice to customers at account opening (GDPR Article 13)
- **Content**: Identity of controller, purposes of processing, legal basis, retention periods, data subject rights, security measures

**IS Impact**:
- Privacy notice published on website and provided at account opening
- Periodic updates to privacy notice (with customer notification if material changes)

##### 3.6.2.2 Security Commitments
- **Contractual Clause**: EuroTrust Bank AG commits to implementing appropriate technical and organizational measures to protect customer data
- **Reference**: General commitment aligned with GDPR Article 32 (no specific controls disclosed to avoid security risks)

**IS Impact**:
- Obligation to maintain information security controls aligned with contractual commitments
- Potential liability for breach of contract in case of data breach due to inadequate security

##### 3.6.2.3 Incident Notification to Customers
- **Obligation**: Notify customers of personal data breaches if high risk to rights and freedoms (GDPR Article 34)
- **Timeframe**: Without undue delay
- **Content**: Description of breach, likely consequences, measures taken, contact point

**IS Impact**:
- Customer notification procedures in incident response plan
- Communication templates for breach notifications (reviewed by Legal and DPO)

##### 3.6.2.4 Data Subject Rights
- **Contractual Basis**: Customers have rights under GDPR (access, rectification, erasure, portability, restriction, objection)
- **Obligation**: EuroTrust Bank AG must facilitate exercise of these rights

**IS Impact**:
- Technical capabilities to fulfill data subject requests (data extraction, deletion, portability)
- Documented procedures for data subject access requests (DSARs)
- Timelines: Response within 1 month of request

##### 3.6.2.5 Consent for Marketing
- **Obligation**: Obtain explicit consent for electronic marketing (ePrivacy Directive, national laws)
- **Mechanism**: Opt-in consent at account opening or via online channels

**IS Impact**:
- Consent management platform (integrated with CRM)
- Opt-out mechanisms (unsubscribe links, preference centres)
- Audit trail of consents and withdrawals

##### 3.6.2.6 Third-Party Data Sharing
- **Disclosure**: Privacy notice discloses categories of third parties with whom data may be shared (e.g., payment processors, credit bureaus, regulators)
- **Safeguards**: Contractual protections and security measures for third-party sharing

**IS Impact**:
- Data sharing agreements with third parties (e.g., credit bureaus, payment networks)
- Encryption of data in transit to third parties
- Access controls for third-party access to customer data

#### 3.6.3 Compliance Status
- **Status**: Compliant
- **Privacy Notice**: Last updated November 2025
- **Customer Consent**: Managed via CRM (Salesforce)

#### 3.6.4 Responsible Department/Role
- **Primary Owner**: Data Protection Officer (DPO)
- **Supporting**: Legal, Compliance, IT, Marketing
- **Customer Communications**: Customer Service & Marketing

---

### 3.7 Non-Disclosure Agreements (NDAs) and Confidentiality Agreements

#### 3.7.1 Overview
- **Purpose**: Protect confidential information shared with third parties (vendors, consultants, auditors, business partners, potential M&A counterparties)
- **Standard Forms**: Unilateral NDA (EuroTrust Bank AG discloses to third party), mutual NDA (both parties disclose)

#### 3.7.2 Key Information Security Obligations

##### 3.7.2.1 Definition of Confidential Information
- **Scope**: Customer data, financial information, business strategies, technical documentation, source code, security policies, intellectual property
- **Exclusions**: Publicly available information, information independently developed, information disclosed by law

##### 3.7.2.2 Obligations of Receiving Party
- **Confidentiality**: Receiving party must keep confidential information secret
- **Use Limitation**: Use only for specified purpose (e.g., providing services, conducting audit)
- **Protection**: Implement reasonable security measures to protect confidential information
- **Disclosure Restriction**: Do not disclose to third parties without consent (exceptions: employees/contractors on need-to-know basis, legal obligations)

**IS Impact**:
- Vendor access controls (limit access to confidential information)
- Secure data transmission methods (encrypted email, secure file transfer)
- Monitoring of third-party access (audit logs)

##### 3.7.2.3 Return or Destruction of Confidential Information
- **Obligation**: Upon termination of NDA or upon request, receiving party must return or destroy confidential information
- **Certification**: Receiving party may be required to certify destruction

**IS Impact**:
- Data offboarding procedures for vendors and partners
- Secure data deletion (e.g., cryptographic erasure, physical destruction of media)

##### 3.7.2.4 Breach Notification
- **Obligation**: Receiving party must notify EuroTrust Bank AG immediately upon discovery of unauthorized disclosure or breach
- **Remediation**: Receiving party must cooperate in remediation

**IS Impact**:
- NDA breach is treated as security incident
- Incident response procedures for third-party data breaches
- Potential legal action for breach of NDA

##### 3.7.2.5 Term and Survival
- **Typical Terms**: 
  - NDA term: 2-5 years
  - Confidentiality obligations survive termination (perpetual or 5-7 years)

**IS Impact**:
- Tracking of NDA expirations and renewals
- Continued protection of confidential information after contract termination

#### 3.7.3 Compliance Status
- **Status**: Compliant
- **NDA Repository**: Maintained by Legal (contract management system)
- **Active NDAs**: ~150 active NDAs with third parties

#### 3.7.4 Responsible Department/Role
- **Primary Owner**: Legal Counsel
- **Supporting**: Procurement, CISO
- **Execution**: Business units (with Legal approval)

---

### 3.8 Cyber Insurance Policy

#### 3.8.1 Contract Information
- **Insurance Provider**: [Example: Allianz Cyber Insurance, AIG CyberEdge] (fictional)
- **Policy Type**: Cyber Liability Insurance + Business Interruption
- **Policy Limit**: €50 million per occurrence
- **Annual Premium**: €2 million (fictional)
- **Policy Period**: 1 January 2026 - 31 December 2026
- **Coverage**: Data breach response costs, regulatory fines (where insurable), business interruption, cyber extortion, legal defense

#### 3.8.2 Key Information Security Obligations

##### 3.8.2.1 Pre-Condition: Security Controls
- **Application Requirement**: Insurer requires evidence of security controls as pre-condition for coverage
- **Due Diligence Questionnaire**: Detailed questionnaire on cybersecurity practices (MFA, encryption, patching, incident response, backups)

**IS Impact**:
- Annual renewal questionnaire (completed by CISO)
- Evidence of security controls (policies, certifications, audit reports)
- Potential premium adjustments based on security posture

##### 3.8.2.2 Notification of Incidents
- **Obligation**: Notify insurer promptly of cyber incidents that may give rise to a claim
- **Timeframe**: As soon as practicable (typically within 72 hours of discovery)
- **Channel**: Insurer's claims hotline or designated contact

**IS Impact**:
- Integration of insurer notification into incident response procedures
- Coordination between incident response team and insurer's breach response services

##### 3.8.2.3 Cooperation with Insurer
- **Obligation**: Cooperate with insurer's investigation of claim
- **Breach Response Vendors**: Insurer may require use of pre-approved vendors (forensic investigators, legal counsel, PR firms)

**IS Impact**:
- Use of insurer's breach response panel (forensic firms, legal firms)
- Documentation of incident response activities for insurer

##### 3.8.2.4 Maintenance of Security Controls
- **Ongoing Obligation**: Maintain security controls represented in insurance application throughout policy period
- **Material Changes**: Notify insurer of material changes to security controls (e.g., termination of MFA, migration to new cloud provider)

**IS Impact**:
- Obligation to maintain security baseline
- Risk of coverage denial if controls deteriorate without notification

##### 3.8.2.5 Regulatory Fines Coverage (Limited)
- **Coverage**: Some regulatory fines may be covered (where insurable under applicable law)
- **Exclusions**: GDPR fines may not be fully insurable in some jurisdictions (public policy considerations)

**IS Impact**:
- Understanding of coverage limitations
- Financial provisioning for uninsured portions of regulatory fines

#### 3.8.3 Compliance Status
- **Status**: Policy active (renewed January 2026)
- **Last Security Questionnaire**: November 2025 (for 2026 renewal)
- **Claims History**: No claims filed in current policy period

#### 3.8.4 Responsible Department/Role
- **Primary Owner**: Chief Risk Officer (CRO)
- **Supporting**: CISO (security questionnaire), Legal (policy review), Finance (premium payment)
- **Claims Management**: CRO + CISO + Legal

---

### 3.9 Interbank Network Agreements (SEPA, TARGET2, EBA Clearing)

#### 3.9.1 Overview
- **Networks**: 
  - **SEPA**: Single Euro Payments Area (credit transfers, direct debits)
  - **TARGET2**: Trans-European Automated Real-time Gross Settlement Express Transfer System (Eurozone RTGS)
  - **EBA Clearing**: STEP2 (SEPA credit transfers and direct debits), EURO1 (large-value payments)
- **Membership**: EuroTrust Bank AG is direct participant in SEPA, TARGET2, and EBA Clearing

#### 3.9.2 Key Information Security Obligations

##### 3.9.2.1 Operational Security Requirements
- **Availability**: Participants must ensure availability of systems to process payments during operating hours
- **Resilience**: Business continuity and disaster recovery capabilities
- **Security Incident Reporting**: Notify network operator of incidents affecting payment processing

**IS Impact**:
- High availability architecture for payment systems (99.9% uptime target)
- DR capabilities (failover to Amsterdam data centre within 4 hours)
- Incident notification procedures to TARGET2, EBA Clearing

##### 3.9.2.2 Compliance with Rulebooks
- **SEPA Rulebook**: Technical specifications for SEPA credit transfers and direct debits (ISO 20022 XML format)
- **TARGET2 Guideline**: ECB guideline governing TARGET2 participation
- **EBA Clearing Rulebooks**: Operational and technical rules for STEP2 and EURO1

**IS Impact**:
- Payment message formatting and validation (ISO 20022 compliance)
- Security of payment message transmission
- Authentication and authorization of payment instructions

##### 3.9.2.3 Certification and Testing
- **Requirement**: Participants must pass certification testing before joining network
- **Ongoing Testing**: Periodic testing of connectivity and message processing (annual or after system changes)

**IS Impact**:
- Testing environments for payment systems
- Change management process (regression testing before production changes)

##### 3.9.2.4 Sanctions and Settlement Risk
- **Obligation**: Participants must screen payments for sanctions compliance
- **Liability**: Participants liable for settlement failures

**IS Impact**:
- Real-time sanctions screening of outgoing payments
- Integration with sanctions lists (OFAC, EU, UN)
- Monitoring of settlement account balances (liquidity management)

##### 3.9.2.5 Security Standards
- **ISO 20022**: Message format standard
- **Digital Signatures**: Certain networks require digital signatures on payment messages (PKI)
- **Encryption**: Secure communication channels (SWIFT, proprietary VPNs)

**IS Impact**:
- PKI infrastructure for digital signatures
- Secure communication channels to network operators (SWIFT Network, dedicated lines)
- Key management for cryptographic operations

#### 3.9.3 Compliance Status
- **Status**: Compliant
- **Last TARGET2 Connectivity Test**: January 2026 (annual test)
- **SEPA Compliance**: Ongoing (monitored by EBA)

#### 3.9.4 Responsible Department/Role
- **Primary Owner**: Head of Treasury & Payments
- **Supporting**: IT, Payments Operations, Compliance
- **Network Connectivity**: IT Infrastructure & Network Engineering

---

### 3.10 Software Licensing Agreements

#### 3.10.1 Overview
- **Scope**: Licenses for commercial software used by EuroTrust Bank AG
- **Key Vendors**: Microsoft (Windows, Office 365, Azure AD), CrowdStrike (endpoint protection), Splunk (SIEM), Salesforce (CRM), Temenos (core banking), Qualys (vulnerability management), Palo Alto Networks (firewalls)

#### 3.10.2 Key Information Security Obligations

##### 3.10.2.1 License Compliance
- **Obligation**: Use software only in accordance with license terms (user count, geographic restrictions, usage restrictions)
- **Audit Rights**: Vendors have right to audit license compliance

**IS Impact**:
- Software asset management (SAM) program
- Tracking of licenses and usage (Microsoft 365 licenses, Splunk data ingestion)
- Annual license true-up exercises

##### 3.10.2.2 Security Configurations
- **Vendor Guidance**: Vendors provide security hardening guides and best practices
- **Obligation**: Implement recommended security configurations

**IS Impact**:
- Configuration management (baseline security configurations)
- Security hardening of operating systems (Windows, Linux)
- Application security settings (e.g., Splunk role-based access control, Salesforce security settings)

##### 3.10.2.3 Patch Management
- **Vendor Obligation**: Provide security patches for vulnerabilities
- **Customer Obligation**: Apply patches in timely manner

**IS Impact**:
- Vulnerability management and patch management programs
- Testing of patches in non-production environments before production deployment
- Emergency patching process for critical vulnerabilities

##### 3.10.2.4 Support and Maintenance Agreements
- **Included Services**: Software updates, security patches, technical support
- **SLAs**: Response times for support tickets (based on severity)

**IS Impact**:
- Maintenance windows for software updates
- Coordination with vendors for major upgrades (e.g., Windows Server upgrades, Temenos core banking upgrades)

##### 3.10.2.5 Data Protection and Privacy
- **Cloud-Based Software** (e.g., Microsoft 365, Salesforce): Data Processing Agreements (DPAs) and Standard Contractual Clauses (SCCs)
- **Data Residency**: Ensure customer data remains in EU regions

**IS Impact**:
- Review of DPAs with SaaS vendors
- Configuration of data residency settings (e.g., Microsoft 365 tenant in EU, Salesforce instance in EU)

##### 3.10.2.6 End-of-Life (EOL) and End-of-Support (EOS)
- **Vendor Announcements**: Vendors announce EOL/EOS dates for products
- **Obligation**: Migrate to supported versions before EOL/EOS

**IS Impact**:
- Tracking of EOL/EOS dates
- Upgrade projects (e.g., Windows Server 2012 EOL → migrate to Windows Server 2022)
- Risk assessments for systems running unsupported software (if migration delayed)

#### 3.10.3 Compliance Status
- **Status**: Compliant
- **Last SAM Audit**: Q4 2025 (internal audit)
- **License Management Tool**: ServiceNow Software Asset Management module

#### 3.10.4 Responsible Department/Role
- **Primary Owner**: Chief Information Officer (CIO) / IT Procurement
- **Supporting**: IT Operations, CISO, Finance
- **Software Asset Management**: IT Asset Management team

---

## 4. Cross-Cutting Themes

### 4.1 Right to Audit
- **Prevalence**: Most contracts include audit rights (or rely on third-party audit reports)
- **Implementation**: Annual review of vendor audit reports (SOC 2, ISO 27001); occasional on-site audits for high-risk vendors
- **Regulator Audit Rights**: Many contracts include provision for regulators to audit service providers

### 4.2 Incident Notification
- **Overlapping Obligations**: Multiple contracts require incident notification (AWS, PCI DSS, SWIFT, correspondents, insurers)
- **Coordination**: Centralized incident response process with notification matrix mapping incidents to contractual obligations

### 4.3 Data Protection and Privacy
- **GDPR Compliance**: DPAs and SCCs required for most third-party relationships involving personal data processing
- **Data Residency**: EU data residency required for customer personal data (contractual and regulatory obligation)

### 4.4 Business Continuity
- **Vendor BCP/DR**: Contracts require vendors to maintain BCP/DR capabilities
- **Testing**: Annual DR testing (internal and with critical vendors)

### 4.5 Exit Planning
- **Standard Clause**: Most contracts include exit provisions (transition assistance, data return/deletion)
- **Implementation**: Documented exit plans for critical outsourcing arrangements (AWS, core banking, payment systems)

---

## 5. Contractual Obligations Register (Summary)

| Contract | Counterparty | Key Obligations | Notification Timelines | Review Frequency | Owner |
|----------|-------------|----------------|----------------------|------------------|-------|
| AWS | Amazon Web Services | Data residency, encryption, SCCs, incident notification, audit reports | Without undue delay | Annually | CIO/CISO |
| PCI DSS | Payment brands (Mastercard/Visa) | Cardholder data protection, quarterly scans, annual assessment, breach notification | Immediate (breach) | Quarterly (scans), Annually (QSA) | Head of Payments |
| SWIFT CSP | SWIFT | 21 mandatory controls, annual attestation, incident reporting, KYC sharing | As soon as possible | Annually | Head of Treasury |
| Correspondent Banking | Multiple banks | Security questionnaires, SWIFT CSP attestation, incident notification | Incident-dependent | Ongoing | Head of Treasury |
| Outsourcing (EBA) | Various vendors | Security clauses, audit rights, incident notification, exit planning | Incident-dependent | Annually (per vendor) | Procurement/CISO |
| Customer Contracts | Retail/corporate customers | Data protection, security measures, breach notification, data subject rights | 72 hours (GDPR breach to regulator), ASAP to customers | Ongoing | DPO/Legal |
| NDAs | Third parties | Confidentiality, security measures, breach notification, data return | Immediate (breach) | Upon expiration | Legal |
| Cyber Insurance | Insurer | Maintain security controls, incident notification, cooperation | 72 hours (claim) | Annually (renewal) | CRO |
| Interbank Networks | SEPA, TARGET2, EBA Clearing | Availability, security, incident reporting, rulebook compliance | Incident-dependent | Ongoing | Head of Treasury |
| Software Licenses | Microsoft, CrowdStrike, Splunk, etc. | License compliance, security configurations, patching, DPAs | N/A | Annually (SAM) | CIO |

---

## 6. Compliance Governance

### 6.1 Contract Management
- **Centralized Repository**: All contracts stored in contract management system (Ironclad) (fictional example)
- **Ownership**: Legal Counsel maintains contract repository
- **Access**: Compliance, CISO, CRO, Procurement have access

### 6.2 Contractual Obligation Tracking
- **Register**: Contractual obligations extracted and tracked in compliance register (see Requirements Register document)
- **Monitoring**: Compliance team monitors adherence to contractual obligations
- **Escalation**: Non-compliance escalated to relevant business owner and executive management

### 6.3 Contract Review Process
- **New Contracts**: Legal and CISO review all new contracts with information security implications
- **Renewals**: Contracts reviewed upon renewal (opportunity to renegotiate security clauses)
- **Amendments**: Material amendments reviewed by Legal and relevant stakeholders

### 6.4 Third-Party Risk Management
- **Integration**: Contractual obligations integrated into vendor risk management program
- **Due Diligence**: Pre-contract due diligence includes security assessment
- **Ongoing Monitoring**: Quarterly business reviews with critical vendors (contractual performance, security posture)

---

## 7. Document Maintenance

### 7.1 Review Schedule
- **Frequency**: Semi-annually (or upon material contract change)
- **Next Scheduled Review**: July 2026
- **Owner**: Chief Compliance Officer + Chief Legal Officer

### 7.2 Change Process
- New contracts executed → Legal extracts security obligations → Update contractual requirements document → Update requirements register → Communicate to relevant owners

---

## Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Legal & Compliance Teams | Initial version for ISO 27001 audit |

---

**END OF DOCUMENT**

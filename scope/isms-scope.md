# ISMS Scope — ISO 27001:2022 Clause 4.3

**Document Reference:** ETB-ISMS-DOC-004.3  
**Version:** 1.0  
**Date:** 14 February 2026  
**Author:** CISO Office, EuroTrust Bank AG  
**Reviewer:** Chief Risk Officer  
**Approver:** Chief Information Security Officer  
**Classification:** Internal Use Only

---

## Document Control

### Change History

| Version | Date | Author | Description of Changes | Approved By |
|---------|------|--------|------------------------|-------------|
| 1.0 | 14-Feb-2026 | CISO Office | Initial release of ISMS Scope document | CISO |

---

## 1. Purpose

This document defines the **scope of the Information Security Management System (ISMS)** for **EuroTrust Bank AG** in accordance with **ISO/IEC 27001:2022 Clause 4.3 – Determining the Scope of the Information Security Management System**.

The purpose of this document is to:

- Clearly define the boundaries and applicability of the ISMS
- Identify the organizational units, locations, assets, processes, and technologies covered by the ISMS
- Document exclusions from the scope with appropriate justification
- Provide a reference point for internal and external audits, certification, and stakeholder communication

---

## 2. Organizational Context

**Organization Name:** EuroTrust Bank AG  
**Headquarters:** Frankfurt, Germany  
**Industry:** Banking and Financial Services  
**Legal Form:** Aktiengesellschaft (AG) — German stock corporation  
**Regulatory Oversight:** BaFin (Bundesanstalt für Finanzdienstleistungsaufsicht), ECB/SSM (European Central Bank / Single Supervisory Mechanism)

**Mission:** To provide secure, reliable, and innovative banking services to retail and corporate customers across Europe while maintaining the highest standards of information security, data protection, and regulatory compliance.

**Note:** EuroTrust Bank AG is a fictional entity created for ISO 27001 training and audit simulation purposes.

---

## 3. ISMS Scope Definition

### 3.1 Scope Statement

The Information Security Management System (ISMS) of **EuroTrust Bank AG** applies to:

> **All information security processes, controls, and technologies supporting the delivery of retail and corporate banking services across EuroTrust Bank AG's European operations, including headquarters and branch locations, IT infrastructure, applications, data centers, cloud services, and third-party service providers critical to the bank's operations.**

---

## 4. Included Elements

### 4.1 Organizational Units

The following organizational units are **included** within the ISMS scope:

| Unit | Description |
|------|-------------|
| **Executive Management (Vorstand)** | Chief Executive Officer (CEO), Chief Financial Officer (CFO), Chief Risk Officer (CRO), Chief Information Security Officer (CISO), Chief Operations Officer (COO) |
| **Information Security Office** | CISO Office, Information Security Managers, Security Operations Center (SOC), Incident Response Team (CSIRT) |
| **IT Department** | IT Operations, Infrastructure Management, Application Development, Database Administration, Network Operations, Cloud Services Management (~200 staff) |
| **Risk Management** | Enterprise Risk Management, Operational Risk, IT Risk, Business Continuity Management |
| **Compliance Department** | Regulatory Compliance, Anti-Money Laundering (AML), Know Your Customer (KYC), Legal Compliance |
| **Data Protection Office** | Data Protection Officer (DPO), Data Privacy Team, GDPR Compliance |
| **Internal Audit** | ISMS Audit, IT Audit, Operational Audit |
| **Human Resources** | Employee Lifecycle Management, Security Awareness & Training, Background Checks |
| **Retail Banking Operations** | Retail customer accounts, payments, loans, mortgages, cards, online/mobile banking (~2 million customers) |
| **Corporate Banking Operations** | Corporate accounts, treasury services, trade finance, corporate lending (~10,000 corporate clients) |
| **Customer Service & Call Centers** | Customer support, helpdesk, complaints management |
| **Facilities & Physical Security** | Data centers, office buildings, physical access control, environmental controls |

### 4.2 Geographic Locations

All EuroTrust Bank AG locations are **included** within the ISMS scope:

| Location | Type | Address (Fictional) | Key Functions |
|----------|------|---------------------|---------------|
| **Frankfurt, Germany** | Headquarters | Taunusanlage 12, 60325 Frankfurt am Main | Executive management, CISO Office, IT Operations, Primary Data Center, Retail & Corporate Banking |
| **Paris, France** | Branch | 15 Avenue des Champs-Élysées, 75008 Paris | Retail & Corporate Banking, Customer Service |
| **Amsterdam, Netherlands** | Branch | Herengracht 450, 1017 CA Amsterdam | Retail & Corporate Banking, IT Support Office |
| **Madrid, Spain** | Branch | Paseo de la Castellana 95, 28046 Madrid | Retail & Corporate Banking |
| **Warsaw, Poland** | Branch | Plac Defilad 1, 00-901 Warsaw | Retail & Corporate Banking, Regional IT Support |
| **Dublin, Ireland** | Branch | St. Stephen's Green 25, Dublin 2 | Corporate Banking, Treasury Services |
| **Frankfurt (Eschborn)** | Secondary Data Center | Frankfurter Straße 100, 65760 Eschborn | Disaster Recovery Site, Backup Data Center |

### 4.3 Information Assets

The following categories of information assets are **included** within the ISMS scope:

#### 4.3.1 Customer and Client Data
- Personal identification information (PII) of retail customers (names, addresses, dates of birth, national IDs, passport numbers)
- Corporate client information (company registration, beneficial ownership, financial statements)
- Account information (account numbers, balances, transaction histories)
- Payment card data (PAN, cardholder data) — subject to PCI DSS compliance
- Credit and loan information (credit scores, collateral details, loan agreements)
- Know Your Customer (KYC) and Anti-Money Laundering (AML) documentation

#### 4.3.2 Financial Transaction Data
- SWIFT messages and interbank communications
- SEPA and TARGET2 payment transactions
- Securities trading and settlement data
- Foreign exchange transactions
- Treasury and liquidity management data

#### 4.3.3 Internal Business Information
- Strategic plans and business strategies
- Risk assessments and risk treatment plans
- Financial reports, budgets, and forecasts
- Internal audit reports and compliance documentation
- Board minutes and executive communications
- Employee personal data (HR records, payroll, performance reviews)

#### 4.3.4 Technical and Operational Information
- IT system configurations and network diagrams
- Application source code and development documentation
- Security policies, procedures, and standards
- Incident response logs and forensic evidence
- Vulnerability assessments and penetration test reports
- Backup and disaster recovery documentation

### 4.4 IT Systems and Applications

The following IT systems and applications are **included** within the ISMS scope:

#### 4.4.1 Core Banking Systems
- **Core Banking Platform:** Temenos Transact (on-premises and cloud-hosted components)
- **Payment Processing System:** In-house developed payment gateway integrated with SWIFT, SEPA, and card networks
- **Loan Origination System:** Finastra Loan IQ
- **Customer Relationship Management (CRM):** Salesforce Financial Services Cloud

#### 4.4.2 Digital Banking Channels
- **Online Banking Portal:** Customer-facing web application for account access and transactions
- **Mobile Banking Applications:** iOS and Android apps for retail and corporate customers
- **ATM Network:** 500+ ATMs across 6 countries (owned and outsourced)

#### 4.4.3 Supporting IT Infrastructure
- **Data Centers:** Primary (Frankfurt), Secondary (Eschborn), Cloud Infrastructure (AWS)
- **Network Infrastructure:** Internal LAN/WAN, VPN, firewalls, intrusion detection/prevention systems (IDS/IPS)
- **Identity and Access Management (IAM):** Active Directory, Multi-Factor Authentication (MFA), Privileged Access Management (PAM)
- **Security Systems:** SIEM (Splunk), Endpoint Detection & Response (EDR), Antivirus, Data Loss Prevention (DLP)
- **Backup and Recovery Systems:** Veeam Backup & Replication, AWS S3 backups

#### 4.4.4 Collaboration and Productivity Tools
- **Email System:** Microsoft 365 (Exchange Online)
- **Collaboration Platform:** Microsoft Teams, SharePoint Online
- **Document Management:** Internal document management system (DMS) for policies and procedures

#### 4.4.5 Third-Party and Cloud Services
- **Cloud Service Provider:** Amazon Web Services (AWS) — EC2, S3, RDS, Lambda
- **SWIFT Network:** Connectivity for interbank messaging and payments
- **Payment Card Networks:** Visa and Mastercard acquiring and issuing services
- **External Service Providers:** IT managed services, penetration testing, security consultancy, facilities management

### 4.5 Business Processes

The following business processes are **included** within the ISMS scope:

| Process Category | Key Processes |
|------------------|---------------|
| **Customer Onboarding** | Account opening, KYC/AML verification, identity proofing, document verification |
| **Payment Processing** | Domestic and international payments, SWIFT messaging, SEPA transfers, card transactions |
| **Lending and Credit** | Loan origination, credit assessment, collateral management, loan servicing |
| **Treasury Operations** | Liquidity management, foreign exchange, securities trading, interbank settlements |
| **IT Service Management** | Incident management, change management, problem management, service desk operations |
| **Information Security Management** | Risk assessment, vulnerability management, incident response, security monitoring, access control |
| **Business Continuity & Disaster Recovery** | BCP/DRP planning, testing, crisis management, failover procedures |
| **Compliance & Regulatory Reporting** | Regulatory incident reporting (BaFin, ECB, DPAs), audit coordination, compliance monitoring |
| **Third-Party Risk Management** | Vendor due diligence, contract management, ongoing monitoring, exit management |
| **Data Protection & Privacy** | GDPR compliance, data subject rights, data breach notification, privacy by design |

---

## 5. Excluded Elements

### 5.1 Organizational Units Excluded

The following organizational units are **excluded** from the ISMS scope with justification:

| Excluded Unit | Justification |
|---------------|---------------|
| **Real Estate Management (Non-IT facilities)** | Property acquisition and management functions not directly involved in information processing or IT systems. Physical security of IT facilities is included. |
| **Marketing & Public Relations** | Marketing campaigns and brand management activities do not process sensitive customer data or critical IT systems. Marketing databases with customer data are included in scope. |
| **Canteen & Catering Services** | Food services provided to employees are not relevant to information security. |

### 5.2 Geographic Locations Excluded

No geographic locations are excluded. All EuroTrust Bank AG offices and data centers are within scope.

### 5.3 Systems and Technologies Excluded

| Excluded System/Technology | Justification |
|---------------------------|---------------|
| **Building Management Systems (Non-IT)** | HVAC, lighting, and general building automation systems not connected to IT networks or critical infrastructure. Environmental controls for data centers are included. |
| **Personal Employee Devices (BYOD)** | Employee-owned personal devices used for non-business purposes are excluded. Corporate mobile devices and BYOD devices accessing corporate resources are included. |

### 5.4 Data Categories Excluded

No categories of business-critical or customer data are excluded. All customer, financial, and operational data within EuroTrust Bank AG's business operations are within the scope.

---

## 6. ISMS Boundaries and Interfaces

### 6.1 Internal Boundaries

- The ISMS scope includes all information processing systems and data flows within EuroTrust Bank AG's operational and IT infrastructure.
- Interfaces between in-scope and out-of-scope systems (e.g., building management) are controlled via network segmentation and access controls.

### 6.2 External Boundaries

The ISMS scope includes:

- **Third-party service providers** that process, store, or transmit EuroTrust Bank AG's information or provide critical IT services (e.g., AWS, SWIFT, payment networks, outsourced IT support).
- **Customer-facing interfaces** such as online banking, mobile apps, and ATM networks.
- **Interbank networks** including SWIFT, SEPA, TARGET2, and correspondent banking relationships.

External parties are subject to:
- Contractual security requirements
- Due diligence and risk assessments
- Ongoing monitoring and audit rights
- Incident notification obligations

### 6.3 Regulatory and Compliance Context

The ISMS operates within the regulatory framework established by:

- **BaFin** — German banking supervision (BAIT, MaRisk)
- **ECB/SSM** — European banking supervision
- **National Data Protection Authorities** — GDPR enforcement (Germany, France, Netherlands, Spain, Poland, Ireland)
- **ENISA / National Cybersecurity Authorities** — NIS2 Directive compliance (BSI Germany, ANSSI France, etc.)
- **Industry Standards** — PCI DSS (payment card security), SWIFT Customer Security Programme (CSP)

---

## 7. Applicability of ISO 27001:2022 Requirements

All clauses and controls of **ISO/IEC 27001:2022** are applicable to this ISMS scope, including:

- **Clauses 4-10:** All mandatory ISMS framework requirements (context, leadership, planning, support, operation, performance evaluation, improvement)
- **Annex A Controls:** All 93 controls from ISO/IEC 27002:2022 have been assessed for applicability. Controls deemed applicable are documented in the Statement of Applicability (SoA).

**No clauses or mandatory requirements of ISO 27001:2022 are excluded.**

---

## 8. Rationale for Scope Definition

The scope of the ISMS has been determined based on:

### 8.1 Internal Context (Clause 4.1)
- EuroTrust Bank AG's mission, strategy, and business objectives
- Organizational structure and governance
- Technology landscape and IT infrastructure
- Dependencies on third-party services

### 8.2 Interested Parties (Clause 4.2)
- Requirements and expectations of customers, regulators, employees, shareholders, and business partners
- Regulatory obligations (BaFin, ECB, GDPR, NIS2, PCI DSS, SWIFT CSP)
- Contractual obligations with service providers and correspondents

### 8.3 Risk-Based Approach
- Critical information assets that require protection
- High-risk business processes (payments, lending, customer data management)
- Legal, regulatory, and contractual requirements
- Threats and vulnerabilities relevant to banking operations

### 8.4 Practical Constraints
- Feasibility of implementing consistent controls across all locations
- Resource availability and management commitment
- Integration with existing risk management and compliance frameworks

---

## 9. Communication and Availability

This ISMS Scope document is:

- **Available** to all employees via the internal document management system (DMS)
- **Communicated** to relevant interested parties including:
  - Executive management and Board
  - Internal audit and compliance functions
  - External auditors and ISO 27001 certification body
  - Regulatory authorities (upon request)
  - Third-party service providers (as relevant)

- **Published** in summary form on EuroTrust Bank AG's external website (public version without sensitive details)

---

## 10. Review and Maintenance

### 10.1 Review Frequency

This ISMS Scope document shall be formally reviewed and updated:

- **Annually** during the Management Review process
- **When significant changes occur**, including:
  - Organizational restructuring (mergers, acquisitions, divestitures)
  - New locations, business units, or services
  - Changes in regulatory requirements or legal obligations
  - Significant changes to IT infrastructure or business processes
  - Audit findings or recommendations related to scope definition

### 10.2 Approval Authority

- **Owner:** Chief Information Security Officer (CISO)
- **Approval:** Executive Management (Vorstand)
- **Review Input:** Risk Management, Compliance, IT Operations, Internal Audit

### 10.3 Change Management

All changes to the ISMS scope must be:
1. Documented with justification
2. Assessed for impact on risk assessment, controls, and compliance
3. Approved by the CISO and Executive Management
4. Communicated to relevant stakeholders
5. Updated in related ISMS documentation (SoA, risk register, policies)

---

## 11. Related Documents

- **ETB-ISMS-DOC-004.1:** Context of the Organization (Clause 4.1)
- **ETB-ISMS-DOC-004.2:** Interested Parties Register (Clause 4.2)
- **ETB-ISMS-POL-001:** Information Security Policy
- **ETB-ISMS-DOC-006.1:** Risk Assessment and Treatment Methodology
- **ETB-ISMS-DOC-006.2:** Statement of Applicability (SoA)
- **ETB-ISMS-DOC-005.31:** Legal, Regulatory and Contractual Requirements Register

---

## 12. Approval

This ISMS Scope document has been reviewed and approved by:

| Name | Role | Signature | Date |
|------|------|-----------|------|
| Dr. Stefan Weber | Chief Information Security Officer | *[Digital Signature]* | 14-Feb-2026 |
| Thomas Müller | Chief Executive Officer | *[Digital Signature]* | 14-Feb-2026 |
| Martin Hoffmann | Chief Risk Officer | *[Digital Signature]* | 14-Feb-2026 |

---

**END OF DOCUMENT**

*This document is prepared for educational purposes as part of an ISO 27001 audit training scenario. EuroTrust Bank AG is a fictional entity created for learning purposes.*
# EuroTrust Bank AG — Firm Overview

## Document Control
- **Document ID**: FP-001
- **Version**: 1.0
- **Date**: February 2026
- **Classification**: Internal
- **Owner**: Corporate Communications & Compliance

---

## 1. Introduction

This document provides a comprehensive overview of EuroTrust Bank AG, including its organizational structure, business operations, geographic presence, and IT infrastructure. This overview serves as foundational context for ISO 27001 compliance activities, particularly in relation to Control 5.31 (Legal, statutory, regulatory and contractual requirements).

**Note**: EuroTrust Bank AG is a **fictional entity** created for educational and demonstration purposes related to ISO 27001 audit training.

---

## 2. Firm Identity

### 2.1 Legal Entity Information
- **Legal Name**: EuroTrust Bank Aktiengesellschaft (AG)
- **Trade Name**: EuroTrust Bank AG
- **Legal Form**: Aktiengesellschaft (Stock Corporation under German law)
- **Registration**: Commercial Register (Handelsregister) Frankfurt am Main HRB 123456
- **LEI (Legal Entity Identifier)**: 529900EUROTRUST123456 (fictional)
- **VAT ID**: DE123456789 (fictional)
- **Founded**: 1995
- **Stock Listing**: Publicly traded on Frankfurt Stock Exchange (FRA: EURO) (fictional)

### 2.2 Headquarters
- **Address**: Taunusanlage 12, 60325 Frankfurt am Main, Germany
- **Phone**: +49 69 1234-5678 (fictional)
- **Email**: info@eurotrust-bank.eu (fictional)
- **Website**: www.eurotrust-bank.eu (fictional)

---

## 3. Geographic Presence

EuroTrust Bank AG operates across **six European countries** with a network of branches and offices:

### 3.1 Germany (Headquarters)
- **Location**: Frankfurt am Main
- **Role**: Global headquarters, primary data centre, treasury operations
- **Employees**: ~2,000
- **Branches**: Frankfurt (HQ), Munich, Berlin, Hamburg, Cologne

### 3.2 France
- **Location**: Paris
- **Address**: 8 Rue de la Paix, 75002 Paris (fictional)
- **Role**: Regional hub for Western Europe, wealth management centre
- **Employees**: ~800
- **Branches**: Paris, Lyon, Marseille

### 3.3 Netherlands
- **Location**: Amsterdam
- **Address**: Herengracht 450, 1017 CA Amsterdam (fictional)
- **Role**: Secondary data centre, digital banking innovation hub
- **Employees**: ~600
- **Branches**: Amsterdam, Rotterdam, The Hague

### 3.4 Spain
- **Location**: Madrid
- **Address**: Paseo de la Castellana 95, 28046 Madrid (fictional)
- **Role**: Southern European operations, corporate banking
- **Employees**: ~700
- **Branches**: Madrid, Barcelona, Valencia

### 3.5 Poland
- **Location**: Warsaw
- **Address**: Marszałkowska 142, 00-061 Warsaw (fictional)
- **Role**: Central and Eastern European operations, back-office services
- **Employees**: ~500
- **Branches**: Warsaw, Kraków, Wrocław

### 3.6 Ireland
- **Location**: Dublin
- **Address**: North Wall Quay, Dublin 1, D01 H104 (fictional)
- **Role**: EU regulatory hub, international treasury operations
- **Employees**: ~400
- **Branches**: Dublin

### 3.7 Summary
- **Total Countries**: 6
- **Total Employees**: ~5,000
- **Total Branches/Offices**: 20+

---

## 4. Business Operations & Services

### 4.1 Core Business Lines

#### 4.1.1 Retail Banking
- Personal current and savings accounts
- Consumer loans and mortgages
- Payment cards (debit and credit)
- Personal investment products
- **Customer Base**: ~2 million retail customers across Europe

#### 4.1.2 Corporate Banking
- Business accounts and cash management
- Corporate lending and credit facilities
- Trade finance and documentary credits
- Treasury and FX services
- **Customer Base**: ~10,000 corporate clients (SMEs to large enterprises)

#### 4.1.3 Wealth Management
- Private banking services
- Portfolio management
- Investment advisory
- Estate planning
- **Customer Base**: ~5,000 high-net-worth individuals (HNWI)

#### 4.1.4 Digital Banking
- Mobile banking application (iOS & Android)
- Web banking platform
- API-based banking services for corporate clients
- Open banking (PSD2-compliant APIs)
- Digital wallet integration
- **Active Digital Users**: ~1.5 million

#### 4.1.5 Cross-Border Payments
- SEPA payments (Single Euro Payments Area)
- International wire transfers (SWIFT network)
- Currency exchange services
- TARGET2 participation (Eurozone real-time gross settlement)

### 4.2 Revenue Distribution (FY2025)
- Retail Banking: 35%
- Corporate Banking: 30%
- Wealth Management: 20%
- Transaction & Payment Services: 10%
- Other (Investment & Trading): 5%

---

## 5. Organizational Structure

### 5.1 Executive Leadership
- **Chief Executive Officer (CEO)**: Dr. Klaus Müller (fictional)
- **Chief Financial Officer (CFO)**: Marie Dubois (fictional)
- **Chief Risk Officer (CRO)**: Jan van den Berg (fictional)
- **Chief Information Officer (CIO)**: Carlos García (fictional)
- **Chief Information Security Officer (CISO)**: Anna Kowalska (fictional)
- **Chief Compliance Officer (CCO)**: Patrick O'Connor (fictional)
- **Data Protection Officer (DPO)**: Dr. Sabine Weber (fictional)

### 5.2 Key Departments
- **IT & Technology**: 600 employees
- **Risk Management**: 200 employees
- **Compliance**: 150 employees
- **Information Security**: 80 employees
- **Data Protection & Privacy**: 40 employees
- **Operations**: 1,200 employees
- **Customer Service**: 800 employees
- **Finance & Treasury**: 400 employees
- **Audit**: 100 employees
- **Legal**: 120 employees
- **Human Resources**: 180 employees
- **Marketing & Communications**: 150 employees
- **Business Units**: 1,180 employees

---

## 6. IT Infrastructure & Technology Landscape

### 6.1 Infrastructure Model
**Hybrid Cloud Architecture**:
- **On-Premises**: Critical core banking systems, legacy applications
- **Cloud**: Customer-facing applications, digital banking, analytics, backup/DR

### 6.2 Data Centres

#### 6.2.1 Primary Data Centre
- **Location**: Frankfurt, Germany
- **Type**: Tier III certified facility
- **Ownership**: Owned and operated by EuroTrust Bank AG
- **Functions**: Core banking system, primary databases, internal applications
- **Security**: 24/7 physical security, biometric access control, environmental controls

#### 6.2.2 Secondary Data Centre (DR Site)
- **Location**: Amsterdam, Netherlands
- **Type**: Tier III certified facility
- **Ownership**: Owned and operated by EuroTrust Bank AG
- **Functions**: Disaster recovery, data replication, backup systems
- **RPO**: 1 hour | **RTO**: 4 hours (for critical systems)

### 6.3 Cloud Services

#### 6.3.1 Cloud Provider
- **Primary Provider**: Amazon Web Services (AWS)
- **Regions Used**: 
  - eu-central-1 (Frankfurt)
  - eu-west-1 (Ireland)
  - eu-west-3 (Paris)
- **Services Used**:
  - EC2, S3, RDS (PostgreSQL, Aurora)
  - Lambda, API Gateway (digital banking)
  - CloudFront, Route 53 (content delivery & DNS)
  - GuardDuty, Security Hub, CloudTrail (security & monitoring)
  - AWS Backup, S3 Glacier (backup & archival)

#### 6.3.2 Cloud Workloads
- Digital banking web and mobile applications
- Customer relationship management (CRM) system
- Business intelligence and analytics platform
- Document management system
- Non-production environments (development, testing, UAT)

### 6.4 Core Systems
- **Core Banking System**: Temenos T24 (on-premises, Frankfurt)
- **Payment Processing**: 
  - SWIFT Alliance Access for international payments
  - SEPA processing engine
  - Card processing platform (Mastercard & Visa certified)
- **Customer Channels**:
  - Mobile banking app (native iOS/Android, API-driven)
  - Online banking (responsive web application)
  - Branch banking system
  - ATM network (managed and outsourced)
- **Enterprise Applications**:
  - ERP: SAP S/4HANA (finance, HR, procurement)
  - Identity & Access Management: Microsoft Entra ID (Azure AD)
  - Email & Collaboration: Microsoft 365 (Exchange Online, Teams, SharePoint)
  - SIEM: Splunk Enterprise Security
  - Vulnerability Management: Qualys
  - Endpoint Protection: CrowdStrike Falcon

### 6.5 Network Architecture
- **WAN**: MPLS network connecting all European offices
- **Internet Connectivity**: Dual-provider redundant links at each major site
- **Firewall**: Next-generation firewalls (Palo Alto Networks)
- **DDoS Protection**: Cloudflare Enterprise
- **VPN**: Cisco AnyConnect for remote employee access

### 6.6 IT Security Technologies
- Multi-factor authentication (MFA) for all employee access
- End-to-end encryption for customer communications
- Data-at-rest encryption (AES-256) for all databases
- Data-in-transit encryption (TLS 1.3)
- Security Operations Centre (SOC) operating 24/7/365
- Regular penetration testing (quarterly external, annual internal)
- Vulnerability scanning (continuous automated scanning)
- Security awareness training (mandatory for all employees annually)

---

## 7. Regulatory & Supervisory Landscape

### 7.1 Primary Regulators
- **European Central Bank (ECB)**: Prudential supervision under Single Supervisory Mechanism (SSM)
- **European Banking Authority (EBA)**: EU-wide regulatory standards
- **BaFin (Germany)**: Bundesanstalt für Finanzdienstleistungsaufsicht — national supervisor for Germany
- **ACPR (France)**: Autorité de contrôle prudentiel et de résolution — French banking supervisor
- **DNB (Netherlands)**: De Nederlandsche Bank — Dutch banking supervisor
- **Banco de España (Spain)**: Spanish banking supervisor
- **KNF (Poland)**: Komisja Nadzoru Finansowego — Polish Financial Supervision Authority
- **Central Bank of Ireland**: Irish banking supervisor

### 7.2 Data Protection Authorities
- **EDPB**: European Data Protection Board (EU-wide coordination)
- **BfDI (Germany)**: Bundesbeauftragter für den Datenschutz und die Informationsfreiheit
- **CNIL (France)**: Commission Nationale de l'Informatique et des Libertés
- **AP (Netherlands)**: Autoriteit Persoonsgegevens
- **AEPD (Spain)**: Agencia Española de Protección de Datos
- **UODO (Poland)**: Urząd Ochrony Danych Osobowych
- **DPC (Ireland)**: Data Protection Commission

### 7.3 Industry Memberships
- European Banking Federation (EBF)
- SWIFT (Society for Worldwide Interbank Financial Telecommunication)
- PCI Security Standards Council (as Merchant and Service Provider)
- Euro Banking Association (EBA) — for SEPA and payments
- European Association of Co-operative Banks (EACB)

---

## 8. Customers & Scale

### 8.1 Customer Metrics
- **Retail Customers**: ~2,000,000
  - Active mobile banking users: 1,200,000
  - Active online banking users: 1,500,000
- **Corporate Customers**: ~10,000
  - SMEs: 8,500
  - Large enterprises: 1,500
- **Private Banking/Wealth Management Clients**: ~5,000

### 8.2 Transaction Volumes (Annual, FY2025)
- **Payment Transactions**: ~200 million
  - SEPA Credit Transfers: 120 million
  - Card Payments: 70 million
  - International Wire Transfers: 8 million
  - Other: 2 million
- **Digital Banking Logins**: ~150 million sessions/year
- **Customer Service Interactions**: ~10 million/year

### 8.3 Data Volumes
- **Customer Records**: 2.01 million individuals + 10,000 legal entities
- **Structured Data (Databases)**: ~500 TB
- **Unstructured Data (Documents, Logs)**: ~2 PB
- **Daily Data Growth**: ~5 TB/day
- **Backup Data**: ~5 PB (including historical backups)

---

## 9. Information Security & Privacy Context

### 9.1 Information Security Management System (ISMS)
- **Standard**: ISO/IEC 27001:2022 (certification target)
- **Scope**: All information assets, systems, and processes supporting EuroTrust Bank AG's operations across all European locations
- **ISMS Owner**: Chief Information Security Officer (CISO)
- **Certification Body**: TÜV SÜD (target certification body, fictional scenario)

### 9.2 Key Information Assets
1. **Customer Personal Data**: Names, addresses, contact details, national IDs, financial information
2. **Payment & Transaction Data**: Account numbers, card details (PCI DSS scope), transaction history
3. **Authentication Credentials**: Passwords, biometric data, MFA tokens
4. **Intellectual Property**: Proprietary banking software, algorithms, business strategies
5. **Internal Communications**: Emails, documents, contracts
6. **System & Application Code**: Source code for banking applications
7. **Security Infrastructure**: Security policies, incident logs, vulnerability reports
8. **Third-Party Data**: Supplier contracts, partner agreements

### 9.3 Data Classification Levels
- **Top Secret**: Board-level strategic documents, M&A information
- **Confidential**: Customer personal data, financial records, security configurations
- **Internal**: Internal policies, procedures, non-sensitive business information
- **Public**: Marketing materials, public website content

---

## 10. Third-Party Relationships

### 10.1 Critical Service Providers
1. **AWS** (Cloud Infrastructure Provider)
2. **Microsoft** (Office 365, Azure AD)
3. **SWIFT** (International payments messaging)
4. **Temenos** (Core banking system support & maintenance)
5. **Mastercard & Visa** (Card payment processing)
6. **CrowdStrike** (Endpoint security)
7. **Cloudflare** (DDoS protection, CDN)
8. **Splunk** (SIEM)
9. **PwC / Deloitte** (External audit services, fictional)
10. **Local data centre facility management companies** (colocation partners)

### 10.2 Outsourced Functions
- ATM network management
- Customer call centre (tier 1 support) — outsourced to Poland
- Certain back-office document processing
- Physical mail processing
- Facilities management at some branch locations

---

## 11. Business Continuity & Disaster Recovery

### 11.1 Objectives
- **RTO (Recovery Time Objective)**: 
  - Tier 1 systems (core banking): 4 hours
  - Tier 2 systems (digital banking): 8 hours
  - Tier 3 systems (internal tools): 24 hours
- **RPO (Recovery Point Objective)**:
  - Tier 1 systems: 1 hour
  - Tier 2 systems: 4 hours
  - Tier 3 systems: 24 hours

### 11.2 DR Strategy
- Active-passive replication between Frankfurt and Amsterdam data centres
- Cloud-based backup for non-core systems (AWS S3 Glacier)
- Annual DR tests and tabletop exercises
- Crisis management team with 24/7 on-call rotation

---

## 12. Key Risks & Threat Landscape

### 12.1 Primary Information Security Risks
1. **Cyber Attacks**: Ransomware, DDoS, phishing, business email compromise
2. **Data Breaches**: Unauthorized access to customer personal data or financial data
3. **Insider Threats**: Malicious or negligent employees, privilege abuse
4. **Third-Party Risks**: Supply chain attacks, vendor security failures
5. **Regulatory Non-Compliance**: GDPR violations, PSD2 non-compliance, breach of NIS2/DORA obligations
6. **System Availability**: Outages impacting customer-facing services
7. **Fraud**: Payment fraud, identity theft, account takeover

### 12.2 Recent Threat Intelligence (Fictional)
- Increase in targeted phishing campaigns against European banks
- APT groups targeting financial sector (e.g., FIN7, Carbanak)
- Ransomware-as-a-service targeting financial institutions
- Regulatory focus on operational resilience (DORA enforcement upcoming)

---

## 13. Strategic Priorities (2026–2028)

### 13.1 Information Security Priorities
1. **Achieve ISO 27001:2022 certification** (Target: Q4 2026)
2. **Full DORA compliance** (Mandatory by January 2025 — ongoing monitoring)
3. **Zero Trust Architecture** implementation (3-year roadmap)
4. **Enhanced threat detection & response** (SOC maturity improvement)
5. **Supply chain security** (Third-party risk management program)

### 13.2 Business Priorities
1. Digital transformation (mobile-first strategy)
2. Expansion of open banking services (API monetization)
3. ESG (Environmental, Social, Governance) integration
4. Customer experience enhancement
5. Operational efficiency through automation

---

## 14. Conclusion

EuroTrust Bank AG is a pan-European banking institution with significant information security and compliance obligations stemming from its operations across six EU member states. The firm's hybrid IT infrastructure, extensive customer base, and diverse service offerings create a complex regulatory landscape requiring rigorous adherence to legal, statutory, regulatory, and contractual requirements as mandated by ISO/IEC 27002:2022 Control 5.31.

This overview serves as the foundation for subsequent compliance documentation and audit activities.

---

## Document Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | February 2026 | Compliance Team | Initial version for ISO 27001 audit |

---

**END OF DOCUMENT**

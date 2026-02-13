# ISO 27001 Audit Project — EuroTrust Bank AG

## 📋 Overview

This repository contains comprehensive documentation for an **ISO/IEC 27001:2022** audit project focused on a fictional European banking institution, **EuroTrust Bank AG**. The project demonstrates practical application of ISO 27001 and ISO 27002 information security management principles in a realistic banking context.

**⚠️ Important Note**: **EuroTrust Bank AG is a fictional entity** created for educational and demonstration purposes. All information, including company details, personnel, systems, and compliance status, is entirely fictional and designed to illustrate ISO 27001 audit practices.

---

## 🏦 About EuroTrust Bank AG (Fictional)

**EuroTrust Bank AG** is an imaginary pan-European banking institution serving as the subject of this ISO 27001 audit demonstration.

### Key Facts
- **Headquarters**: Frankfurt, Germany
- **Geographic Presence**: 6 EU countries (Germany, France, Netherlands, Spain, Poland, Ireland)
- **Employees**: ~5,000 across Europe
- **Customers**: ~2 million retail customers and ~10,000 corporate clients
- **Services**: Retail banking, corporate banking, wealth management, digital banking, cross-border payments
- **IT Infrastructure**: Hybrid cloud (on-premises data centres in Frankfurt & Amsterdam + AWS EU regions)
- **Regulatory Environment**: Supervised by ECB (SSM), BaFin, and national authorities in 6 countries

For full details, see [`firm-profile/firm-overview.md`](firm-profile/firm-overview.md).

---

## 🎯 Project Objective

This project focuses on **ISO/IEC 27002:2022 Control 5.31** (formerly A.18.1.1 in ISO 27001:2013):

> **Control 5.31 — Legal, statutory, regulatory and contractual requirements**
> 
> *"Requirements relevant to information security arising from legal, statutory, regulatory and contractual obligations should be identified, documented and kept up to date. The organization's approach to meeting these requirements should also be identified and documented."*

The documentation demonstrates how a European bank identifies, catalogues, and manages the complex web of legal, regulatory, and contractual obligations applicable to its information security management system (ISMS).

---

## 📁 Repository Structure

```
iso-documents/
├── README.md                                    # This file
├── firm-profile/
│   └── firm-overview.md                         # EuroTrust Bank AG company profile
├── legal-and-regulatory-requirements/
│   ├── eu-wide-regulations.md                   # EU-wide regulations (GDPR, PSD2, DORA, NIS2, etc.)
│   ├── country-specific-regulations.md          # National laws (Germany, France, NL, Spain, Poland, Ireland)
│   ├── contractual-requirements.md              # Contractual obligations (AWS, PCI DSS, SWIFT, etc.)
│   ├── requirements-register.md                 # Consolidated register of 82 requirements
│   └── compliance-approach.md                   # Firm's approach to meeting requirements
└── [Additional ISO 27001 reference materials]   # Supporting PDFs
```

---

## 📚 Documentation Contents

### 1. Firm Profile

#### [`firm-profile/firm-overview.md`](firm-profile/firm-overview.md)
Comprehensive profile of EuroTrust Bank AG including:
- Legal entity information and corporate structure
- Geographic presence (6 countries, 20+ branches)
- Business operations (retail, corporate, wealth management, digital banking)
- Organizational structure and executive leadership
- IT infrastructure (hybrid cloud architecture, data centres, core systems)
- Regulatory landscape and supervisory relationships
- Customer base and transaction volumes (200M+ transactions annually)
- Information security context

---

### 2. Legal & Regulatory Requirements

#### [`legal-and-regulatory-requirements/eu-wide-regulations.md`](legal-and-regulatory-requirements/eu-wide-regulations.md)

Detailed documentation of **10 EU-wide regulations** applicable to the bank's information security:

1. **GDPR** (Regulation EU 2016/679) — Data protection principles, security of processing, breach notification, DPIAs
2. **PSD2** (Directive EU 2015/2366) — Strong customer authentication, protection of credentials, incident reporting
3. **DORA** (Regulation EU 2022/2554) — ICT risk management, incident management, testing, third-party risk
4. **NIS2 Directive** (Directive EU 2022/2555) — Cybersecurity risk management, incident reporting, governance
5. **eIDAS** (Regulation EU 910/2014) — Electronic signatures, trust services
6. **EBA Guidelines on ICT** (EBA/GL/2019/04) — IT governance, security, third-party risk, business continuity
7. **ECB/SSM Cyber Resilience Expectations** — Threat intelligence, penetration testing, TLPT
8. **AMLD 5 & 6** (Directives EU 2018/843 & 2018/1673) — AML internal controls, data protection for AML
9. **MiFID II** (Directive 2014/65/EU) — IT security for investment services, record-keeping
10. **ePrivacy Directive** (Directive 2002/58/EC) — Confidentiality of communications, cookie consent

For each regulation:
- Full legal reference and citation
- Scope and applicability
- Key information security obligations (with article references)
- Compliance status and responsible owners
- Review frequency

---

#### [`legal-and-regulatory-requirements/country-specific-regulations.md`](legal-and-regulatory-requirements/country-specific-regulations.md)

National laws and regulations for each of the **6 countries** where EuroTrust Bank operates:

##### **Germany** (Headquarters)
- **BDSG** (Federal Data Protection Act) — Employee data protection, DPO
- **KWG** (Banking Act, Section 25a/b) — IT systems security, outsourcing
- **BAIT** (BaFin IT Requirements) — ISMS, user access management, DR, network management
- **IT-SiG 2.0** (IT Security Act 2.0) — Critical infrastructure security, incident reporting to BSI

##### **France**
- **Loi Informatique et Libertés** — French GDPR implementation
- **ACPR Guidelines** — IT governance, BCP, outsourcing
- **LPM** (Military Programming Law) — Critical infrastructure (OIV designation)

##### **Netherlands**
- **UAVG** — Dutch GDPR implementation
- **DNB Good Practices** — IT governance, operational resilience (Amsterdam DC), third-party risk
- **Wbni** (NIS Implementation Act) — Cybersecurity, incident reporting

##### **Spain**
- **LOPDGDD** (Organic Law 3/2018) — Data protection, digital rights, employee monitoring
- **Banco de España Circulars** — IT governance, BCP, outsourcing

##### **Poland**
- **National Cybersecurity System Act** — Cybersecurity risk management, incident reporting, audits
- **KNF Recommendations** — IT risk management

##### **Ireland**
- **Data Protection Act 2018** — Irish GDPR implementation
- **CBI Cross Industry Guidance** — IT governance, operational resilience, third-party risk

---

#### [`legal-and-regulatory-requirements/contractual-requirements.md`](legal-and-regulatory-requirements/contractual-requirements.md)

Detailed analysis of **10 categories of contractual obligations**:

1. **AWS (Cloud Service Provider)** — Data processing agreement, SCCs, shared responsibility model, security incident notification, audit rights, SLAs
2. **PCI DSS** (Payment Card Industry) — 12 requirements covering cardholder data security, quarterly scans, annual QSA audit
3. **SWIFT Customer Security Programme (CSP)** — 21 mandatory controls, annual attestation, incident reporting, SWIFT environment segregation
4. **Correspondent Banking Agreements** — Security questionnaires, incident notification, audit rights, data protection
5. **Outsourcing Agreements (EBA Guidelines)** — Security clauses, due diligence, regulator notifications, ongoing monitoring
6. **Customer Contracts** — Privacy notices, breach notification, data subject rights, consent management
7. **Non-Disclosure Agreements (NDAs)** — Confidentiality, security measures, breach notification
8. **Cyber Insurance Policy** — Maintain security controls, incident notification, cooperation with insurer
9. **Interbank Networks** (SEPA, TARGET2, EBA Clearing) — Operational security, availability, incident reporting
10. **Software Licensing** — License compliance, security configurations, patching, data residency

---

#### [`legal-and-regulatory-requirements/requirements-register.md`](legal-and-regulatory-requirements/requirements-register.md)

**Consolidated register of 82 individual requirements** in a comprehensive table format, including:

| Column | Description |
|--------|-------------|
| **Req ID** | Unique identifier (EU-01, DE-01, CON-01, etc.) |
| **Category** | Legal, Regulatory, or Contractual |
| **Requirement Name** | Short description |
| **Reference/Source** | Legal citation, regulation number, or contract |
| **Jurisdiction** | EU-wide, specific country, or global |
| **Applicable Business Area** | Affected systems or business functions |
| **Key IS Obligations** | Summary of information security obligations |
| **Compliance Owner** | Responsible department or role |
| **Review Frequency** | How often reviewed (ongoing, quarterly, annually, etc.) |
| **Last Reviewed** | Date of last review |
| **Status** | Compliant, In Progress, or Non-Compliant |

**Summary Statistics**:
- 33 EU-wide regulatory requirements
- 24 country-specific legal/regulatory requirements
- 25 contractual requirements
- **Total: 82 requirements**
- **96% compliant** (79 requirements), 4% in progress (NIS2 transposition)

**Cross-cutting themes** analyzed: incident reporting, third-party risk, encryption, penetration testing, business continuity.

---

#### [`legal-and-regulatory-requirements/compliance-approach.md`](legal-and-regulatory-requirements/compliance-approach.md)

Comprehensive documentation of the firm's **approach to meeting requirements**, including:

1. **Governance Structure**
   - Three Lines of Defense model
   - Organizational chart (Board → Executive Committee → CCO/CISO/DPO/CRO)
   
2. **Roles & Responsibilities**
   - Board of Directors, Board Risk Committee, Audit Committee
   - CEO, CCO, CISO, CRO, DPO, Chief Legal Officer
   - Country Managers, Business Unit Heads
   - Internal Audit

3. **Process for Identifying New/Changed Requirements**
   - Regulatory horizon scanning (daily monitoring, monthly summaries, quarterly reports)
   - Identification and impact assessment process (6-step methodology)
   - Example: NIS2 Directive implementation process (2022-2026 timeline)

4. **Monitoring and Review Procedures**
   - Compliance monitoring activities (self-assessments, second-line reviews, KRIs, incident monitoring)
   - Compliance testing (design testing, operating effectiveness, penetration testing, DR testing)
   - Internal and external reporting (monthly, quarterly, annually)

5. **Integration with ISMS (ISO 27001)**
   - Mapping to ISO 27001 clauses (4-10)
   - Integration of requirements into risk assessments, controls, monitoring
   - Annex A controls mapped to legal/regulatory requirements

6. **Training and Awareness**
   - Mandatory annual training for all employees (GDPR, PSD2, incident reporting)
   - Role-based training (InfoSec team, Compliance team, IT teams, Payments, Treasury, Country teams)
   - Executive and Board training
   - Awareness campaigns (phishing simulations, newsletters, Data Privacy Day, Cybersecurity Awareness Month)

7. **Record-Keeping and Evidence**
   - Documentation requirements (policies, risk assessments, DPIAs, vendor assessments)
   - Compliance evidence (penetration tests, audit reports, training records, incident reports)
   - Retention periods (10 years for business records, 5 years for transactions, 1-3 years for logs)

8. **Escalation and Incident Response**
   - Compliance breach escalation process (detection → assessment → notification → remediation → lessons learned)
   - Regulatory investigation support

9. **Continuous Improvement**
   - Improvement initiatives (ISO 27001 certification, Zero Trust, GRC tool, automation)

---

## 🔍 Key Highlights

### Comprehensive Scope
- **82 requirements** catalogued across EU-wide regulations, 6 national jurisdictions, and 10 categories of contracts
- **10 EU regulations**, **24 country-specific laws**, **25 contractual obligations**

### Realistic Complexity
- Multi-country operations (6 EU countries)
- Hybrid cloud infrastructure (on-premises + AWS)
- Multiple regulatory supervisors (ECB, BaFin, ACPR, DNB, Banco de España, KNF, CBI, 6 DPAs)
- Complex contractual landscape (PCI DSS, SWIFT CSP, correspondent banks, outsourcing)

### Professional Quality
- Proper legal citations and references (regulation numbers, article numbers, directive numbers)
- Structured documentation with version control and document IDs
- Cross-referencing between documents
- Realistic timelines and compliance status

### Practical Insights
- **Incident reporting complexity**: Overlapping obligations to report to multiple authorities (GDPR 72h, DORA, NIS2 24h/72h/1 month, national laws)
- **Third-party risk management**: Consolidated approach across DORA, EBA Guidelines, national regulations, and contracts
- **Testing requirements**: Annual penetration testing (multiple regulations), TLPT every 3 years, quarterly PCI DSS scans
- **Governance**: Three Lines of Defense model, Board oversight, defined roles (CCO, CISO, DPO, CRO)

---

## 🎓 Educational Use

This project is designed for:
- **ISO 27001 Lead Auditor training** — Understanding Control 5.31 in a complex, multi-jurisdictional environment
- **Information security professionals** — Learning about banking sector compliance
- **Compliance professionals** — Understanding interaction between legal, regulatory, and contractual obligations
- **Risk management professionals** — Seeing integration of compliance into ISMS
- **Banking IT professionals** — Understanding regulatory landscape for European banks

---

## 📖 Standards & Frameworks Referenced

- **ISO/IEC 27001:2022** — Information Security Management Systems
- **ISO/IEC 27002:2022** — Information Security Controls (specifically Control 5.31)
- **ISO 19011:2018** — Guidelines for Auditing Management Systems
- **GDPR** — General Data Protection Regulation (EU 2016/679)
- **PSD2** — Payment Services Directive 2 (EU 2015/2366)
- **DORA** — Digital Operational Resilience Act (EU 2022/2554)
- **NIS2 Directive** — Network and Information Security Directive 2 (EU 2022/2555)
- **EBA Guidelines** — European Banking Authority Guidelines (EBA/GL/2019/04)
- **PCI DSS v4.0** — Payment Card Industry Data Security Standard
- **SWIFT Customer Security Programme (CSP)**
- **National laws and regulations** (Germany: BDSG, KWG, BAIT, IT-SiG 2.0; France: Loi Informatique et Libertés, LPM; etc.)

---

## ⚠️ Disclaimer

**This is a fictional educational project.** 

- **EuroTrust Bank AG does not exist.** All company information, including business operations, systems, personnel names, locations, and contact details, is entirely fictional.
- **Compliance status is illustrative.** The documented compliance status, audit dates, and certifications are fictional and for demonstration purposes only.
- **Regulations and laws are real.** The legal and regulatory references (GDPR, DORA, PSD2, BAIT, etc.) are accurate as of February 2026 (project date), but readers should verify current versions and applicability.
- **Not legal advice.** This documentation does not constitute legal, compliance, or professional advice. Organizations should consult qualified legal counsel and compliance professionals for actual compliance programs.
- **Simplified for clarity.** Real-world compliance is more complex and nuanced than can be fully captured in a demonstration project.

---

## 📅 Project Information

- **Project Creation Date**: February 2026 (fictional scenario date)
- **ISO 27001 Version**: ISO/IEC 27001:2022
- **ISO 27002 Version**: ISO/IEC 27002:2022
- **Target Control**: Control 5.31 — Legal, statutory, regulatory and contractual requirements
- **Document Version**: 1.0
- **Total Pages**: 300+ pages of documentation across 6 documents

---

## 📞 Contact (Fictional)

**EuroTrust Bank AG** (Fictional Entity)
- Website: www.eurotrust-bank.eu (does not exist)
- Email: info@eurotrust-bank.eu (does not exist)
- Address: Taunusanlage 12, 60325 Frankfurt am Main, Germany (fictional address)

**Compliance Contact** (Fictional)
- Chief Compliance Officer: Patrick O'Connor (fictional person)
- Email: compliance@eurotrust-bank.eu (does not exist)

**Information Security Contact** (Fictional)
- Chief Information Security Officer: Anna Kowalska (fictional person)
- Email: infosec@eurotrust-bank.eu (does not exist)

---

## 📄 License

This educational project is provided for demonstration and training purposes. All content is fictional and created for ISO 27001 audit training.

---

## 🙏 Acknowledgments

This project demonstrates the practical application of:
- ISO/IEC 27001:2022 and ISO/IEC 27002:2022 standards
- European Union data protection and cybersecurity regulations
- Banking sector supervisory expectations and industry standards

Created to illustrate best practices in identifying, documenting, and managing legal, regulatory, and contractual requirements for information security in a complex, multi-jurisdictional banking environment.

---

**Last Updated**: February 2026  
**Document Status**: Version 1.0 — Initial Release for ISO 27001 Audit Demonstration

---

*"Information security compliance is not just about checkboxes—it's about building a systematic, sustainable approach to identifying and meeting obligations in an ever-changing regulatory landscape."*

---


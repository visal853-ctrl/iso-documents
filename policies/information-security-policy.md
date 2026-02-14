# Information Security Policy — ISO 27001:2022

**Document Reference:** ETB-ISMS-POL-001  
**Version:** 2.0  
**Date:** 14 February 2026  
**Author:** CISO Office, EuroTrust Bank AG  
**Reviewer:** Chief Risk Officer, Chief Compliance Officer  
**Approver:** Chief Executive Officer, Chief Information Security Officer  
**Classification:** Internal Use Only

---

## Document Control

### Change History

| Version | Date | Author | Description of Changes | Approved By |
|---------|------|--------|------------------------|-------------|
| 1.0 | 01-Jan-2025 | CISO Office | Initial policy establishment | CEO, CISO |
| 2.0 | 14-Feb-2026 | CISO Office | Comprehensive update aligned with ISO 27001:2022 | CEO, CISO |

---

## 1. Executive Summary

This Information Security Policy establishes the strategic direction and principles for information security management at **EuroTrust Bank AG**. This policy demonstrates the commitment of executive management and the Board of Directors to protecting the confidentiality, integrity, and availability of all information assets across the organization.

EuroTrust Bank AG recognizes that information security is fundamental to:
- Maintaining customer trust and confidence
- Meeting regulatory obligations and legal requirements
- Protecting competitive advantage and business operations
- Ensuring operational resilience and business continuity
- Supporting digital innovation while managing risks

This policy applies to all employees, contractors, third parties, and business partners who access, process, store, or transmit EuroTrust Bank AG information.

---

## 2. Purpose and Objectives

### 2.1 Purpose

The purpose of this Information Security Policy is to:

1. Define EuroTrust Bank AG's commitment to information security
2. Establish the framework for the Information Security Management System (ISMS)
3. Set strategic objectives for information security
4. Define roles, responsibilities, and accountability for information security
5. Ensure compliance with ISO/IEC 27001:2022 and applicable legal, regulatory, and contractual requirements

### 2.2 Information Security Objectives

EuroTrust Bank AG is committed to achieving the following information security objectives:

| Objective | Target | Measurement |
|-----------|--------|-------------|
| **Protect Customer Data** | Zero unauthorized disclosures of customer personal data | Number of confirmed data breaches |
| **Maintain System Availability** | 99.9% uptime for critical banking systems | System availability metrics |
| **Regulatory Compliance** | 100% compliance with BaFin, ECB, and GDPR requirements | Audit findings, regulatory assessments |
| **Incident Response** | Detect and respond to security incidents within defined timeframes | Mean time to detect (MTTD), mean time to respond (MTTR) |
| **Security Awareness** | 100% of employees complete annual security awareness training | Training completion rates |
| **Third-Party Security** | All critical vendors meet security requirements | Vendor assessment scores |
| **Risk Management** | All high risks have approved treatment plans | Risk register status |

---

## 3. Scope

This policy applies to:

### 3.1 People
- All EuroTrust Bank AG employees (permanent, temporary, part-time)
- Contractors, consultants, and agency staff
- Third-party service providers and suppliers
- Business partners with access to EuroTrust Bank AG information or systems
- Board members and executive management

### 3.2 Information Assets
- All information regardless of format (electronic, paper, verbal)
- Customer and client data
- Financial transaction data
- Business and operational information
- Technical and IT system data
- Intellectual property and proprietary information

### 3.3 Technology
- All IT systems, applications, and infrastructure
- Network and communication systems
- Cloud services and platforms
- Mobile and remote access technologies
- Physical facilities supporting IT operations

### 3.4 Locations
- All EuroTrust Bank AG offices and branches across Europe
- Data centers (primary and disaster recovery sites)
- Remote work locations
- Third-party facilities processing EuroTrust Bank AG data

---

## 4. Management Commitment and Leadership

### 4.1 Board and Executive Commitment

The Board of Directors and Executive Management (Vorstand) of EuroTrust Bank AG:

✅ **Commit** to establishing, implementing, maintaining, and continually improving the ISMS  
✅ **Ensure** that information security objectives are established and aligned with strategic direction  
✅ **Provide** adequate resources (financial, human, technical) for the ISMS  
✅ **Integrate** information security requirements into business processes  
✅ **Communicate** the importance of effective information security management  
✅ **Support** the CISO and information security team in their responsibilities  
✅ **Promote** a culture of security awareness throughout the organization  
✅ **Ensure** accountability for information security at all levels  

### 4.2 Management Review

Executive management shall conduct formal management reviews of the ISMS at least **quarterly** to:
- Evaluate ISMS performance against objectives
- Review risk assessment outcomes and treatment effectiveness
- Address internal and external changes affecting information security
- Assess opportunities for continual improvement
- Make decisions on resource allocation and strategic direction

---

## 5. Information Security Principles

EuroTrust Bank AG's approach to information security is based on the following core principles:

### 5.1 Confidentiality
Information shall be protected from unauthorized access and disclosure. Access to information is granted on a "need-to-know" and "least privilege" basis.

### 5.2 Integrity
Information shall be accurate, complete, and protected from unauthorized modification or destruction. Changes to information and systems shall be controlled and auditable.

### 5.3 Availability
Information and systems shall be accessible and usable when required by authorized users. Business continuity and disaster recovery capabilities ensure resilience.

### 5.4 Accountability
Individuals and entities are accountable for their information security responsibilities. Actions are logged, monitored, and subject to review.

### 5.5 Compliance
All activities comply with applicable laws, regulations, contractual obligations, and internal policies. Non-compliance is not tolerated.

### 5.6 Risk-Based Approach
Information security decisions are based on risk assessment. Controls are implemented proportionate to the level of risk.

### 5.7 Defense in Depth
Multiple layers of security controls protect information assets. No single point of failure exists.

### 5.8 Privacy by Design
Data protection and privacy requirements are integrated into systems and processes from the outset.

---

## 6. Policy Statements

### 6.1 Asset Management

**Policy:** All information assets shall be identified, classified, and protected according to their value, sensitivity, and criticality to business operations.

**Requirements:**
- Asset inventory maintained for all information assets
- Information classification scheme applied (Public, Internal, Confidential, Restricted)
- Asset ownership assigned with clear accountability
- Handling requirements defined for each classification level
- Media disposal conducted securely (data erasure, physical destruction)

### 6.2 Access Control

**Policy:** Access to information and systems is controlled based on business need, least privilege, and segregation of duties principles.

**Requirements:**
- User access provisioning and de-provisioning procedures
- Multi-factor authentication (MFA) for all remote access and privileged accounts
- Regular access reviews (quarterly for privileged access, annually for standard access)
- Segregation of duties for critical functions
- Privileged access management (PAM) for administrative accounts
- Strong password requirements and password management tools
- Automatic session timeout and screen locking

### 6.3 Cryptography

**Policy:** Cryptographic controls shall be used to protect the confidentiality, integrity, and authenticity of sensitive information.

**Requirements:**
- Encryption of data at rest for all customer personal data and payment card data
- Encryption of data in transit using TLS 1.2 or higher
- Cryptographic key management procedures (generation, storage, rotation, destruction)
- Digital signatures for critical transactions and communications
- Compliance with regulatory requirements (GDPR, PCI DSS)

### 6.4 Physical and Environmental Security

**Policy:** Physical access to facilities containing information assets is controlled and monitored to prevent unauthorized access, damage, and interference.

**Requirements:**
- Physical access control systems (badge readers, biometrics)
- Visitor management and escort procedures
- Video surveillance of critical areas
- Environmental controls (HVAC, fire suppression, power backup)
- Clean desk and clear screen policies
- Secure disposal of physical media and documents

### 6.5 Operations Security

**Policy:** IT operations are managed securely to ensure the correct and secure operation of information processing facilities.

**Requirements:**
- Change management procedures for all system changes
- Capacity management and performance monitoring
- Separation of development, testing, and production environments
- Malware protection on all endpoints and servers
- System backup procedures and restoration testing
- Logging and monitoring of security events
- Vulnerability management and patching (critical patches within 14 days)
- Network segmentation and security controls

### 6.6 Communications Security

**Policy:** Networks and information transfers are secured to protect the confidentiality and integrity of information.

**Requirements:**
- Network security controls (firewalls, IDS/IPS, web filtering)
- Secure network design and segmentation
- Secure configuration of network devices
- Network access control (NAC) for device authentication
- Secure email (encryption, anti-spam, anti-phishing)
- Secure file transfer protocols (SFTP, HTTPS)
- Virtual Private Network (VPN) for remote access

### 6.7 System Acquisition, Development, and Maintenance

**Policy:** Security is integrated into the entire lifecycle of information systems including acquisition, development, testing, and maintenance.

**Requirements:**
- Security requirements defined in system specifications
- Secure development lifecycle (SDLC) practices
- Code review and security testing (SAST, DAST, penetration testing)
- Separation of development and production environments
- Change control and version management
- Security testing before production deployment
- Secure coding guidelines and standards

### 6.8 Supplier Relationships

**Policy:** Information security requirements are established and maintained in relationships with suppliers and third-party service providers.

**Requirements:**
- Vendor due diligence and security assessments before engagement
- Security requirements included in contracts and SLAs
- Right to audit third-party service providers
- Ongoing monitoring and periodic reassessment
- Incident notification obligations
- Data protection agreements (DPAs) for processors of personal data
- Exit management and data return/destruction procedures

### 6.9 Information Security Incident Management

**Policy:** Information security incidents are detected, reported, assessed, responded to, and learned from in a timely and effective manner.

**Requirements:**
- 24/7 security monitoring via Security Operations Center (SOC)
- Incident reporting channels and procedures
- Incident classification and prioritization
- Computer Security Incident Response Team (CSIRT) established
- Incident response procedures and playbooks
- Forensic investigation capabilities
- Regulatory notification within required timeframes (72 hours for GDPR)
- Post-incident review and lessons learned

### 6.10 Business Continuity

**Policy:** Business continuity and disaster recovery capabilities ensure the resilience of critical business functions and information systems.

**Requirements:**
- Business impact analysis (BIA) conducted annually
- Business continuity plans (BCP) for critical business functions
- Disaster recovery plans (DRP) for critical IT systems
- Recovery time objectives (RTO) and recovery point objectives (RPO) defined
- Regular testing of BC/DR plans (annually minimum)
- Redundant systems and failover capabilities
- Data backup and restoration procedures
- Crisis management and communication procedures

### 6.11 Compliance

**Policy:** Information security practices comply with all applicable legal, regulatory, contractual, and internal requirements.

**Requirements:**
- Legal and regulatory requirements register maintained
- Compliance monitoring and reporting
- Internal audits conducted (minimum annually)
- External audits and certifications (ISO 27001, PCI DSS)
- Data protection impact assessments (DPIAs) for high-risk processing
- Records retention and legal hold procedures
- Intellectual property protection
- Privacy and data protection compliance (GDPR)

### 6.12 Human Resources Security

**Policy:** Information security responsibilities are established before, during, and after employment or engagement.

**Requirements:**
- Background checks for all employees (criminal, employment, education verification)
- Confidentiality and non-disclosure agreements (NDAs)
- Security roles and responsibilities in job descriptions
- Security awareness training (mandatory annual training + onboarding)
- Acceptable use policy acknowledgment
- Termination procedures (access revocation within 24 hours)
- Disciplinary process for security violations

### 6.13 Mobile and Remote Working

**Policy:** Information security is maintained when employees work remotely or use mobile devices.

**Requirements:**
- Mobile device management (MDM) for corporate devices
- Device encryption for laptops and mobile devices
- Remote wipe capabilities for lost/stolen devices
- Secure remote access via VPN with MFA
- Acceptable use requirements for remote working
- Physical security of devices and information
- Prohibition of public Wi-Fi for sensitive work (or VPN required)

### 6.14 Cloud Security

**Policy:** Cloud services are selected, configured, and managed securely in accordance with shared responsibility models.

**Requirements:**
- Cloud service provider (CSP) due diligence and security assessment
- Contractual security requirements and SLAs
- Secure configuration of cloud services (AWS best practices)
- Cloud access controls (IAM, MFA, least privilege)
- Data residency and sovereignty considerations
- Cloud security monitoring and logging
- Regular security assessments of cloud environments

---

## 7. Roles and Responsibilities

### 7.1 Board of Directors
- Provide oversight of information security strategy and performance
- Approve information security policy and strategic direction
- Ensure adequate resources for information security
- Review significant security risks and incidents

### 7.2 Chief Executive Officer (CEO)
- Ultimate accountability for information security
- Approve information security policy
- Champion information security culture
- Ensure integration of security into business strategy

### 7.3 Chief Information Security Officer (CISO)
- Overall responsibility for ISMS implementation and operation
- Define information security strategy and roadmap
- Report to executive management and Board on security posture
- Manage information security team and budget
- Coordinate incident response and crisis management
- Interface with regulators and auditors on security matters

### 7.4 Information Security Team
- Implement and maintain security controls
- Monitor security events and investigate incidents
- Conduct risk assessments and security testing
- Provide security guidance and support to business units
- Deliver security awareness training
- Maintain security documentation

### 7.5 Chief Risk Officer (CRO)
- Integrate information security risks into enterprise risk management
- Oversight of risk assessment process
- Review and challenge risk treatment decisions

### 7.6 Data Protection Officer (DPO)
- Ensure GDPR compliance
- Advise on data protection impact assessments
- Coordinate data breach notifications
- Liaise with data protection authorities

### 7.7 IT Department
- Implement technical security controls
- Maintain secure IT infrastructure and systems
- Apply security patches and updates
- Manage user access provisioning
- Conduct system backups
- Support incident response activities

### 7.8 Business Unit Managers
- Ensure compliance with security policies within their areas
- Identify and report security risks
- Support security initiatives and projects
- Ensure employees receive required security training
- Act as information asset owners for business data

### 7.9 All Employees
- Comply with all information security policies and procedures
- Complete required security awareness training
- Report security incidents and suspected vulnerabilities
- Protect information assets and credentials
- Follow acceptable use guidelines
- Challenge unauthorized access or suspicious activities

### 7.10 Internal Audit
- Conduct independent audits of ISMS effectiveness
- Assess compliance with policies and controls
- Report findings to executive management and Board
- Follow up on corrective actions

---

## 8. Compliance and Enforcement

### 8.1 Regulatory and Legal Compliance

EuroTrust Bank AG complies with all applicable information security laws, regulations, and standards including:

- **ISO/IEC 27001:2022** — Information Security Management Systems
- **GDPR (General Data Protection Regulation)** — EU data protection law
- **BaFin BAIT** — German banking IT security requirements
- **MaRisk** — German minimum requirements for risk management
- **ECB/SSM** — European Central Bank supervisory expectations
- **NIS2 Directive** — EU directive on network and information security
- **PCI DSS** — Payment Card Industry Data Security Standard
- **SWIFT Customer Security Programme (CSP)** — Financial messaging security

### 8.2 Policy Compliance

Compliance with this policy is **mandatory** for all persons within scope. Non-compliance may result in:

- Disciplinary action up to and including termination of employment
- Termination of contractor or third-party relationships
- Legal action for breach of confidentiality or data protection laws
- Regulatory sanctions and penalties
- Financial liability for damages

### 8.3 Exceptions

Exceptions to this policy or supporting standards must be:
1. Documented with business justification and risk assessment
2. Approved by the CISO (or CEO for CISO exceptions)
3. Time-limited with defined compensating controls
4. Reviewed regularly for continued validity

### 8.4 Monitoring and Audit

Information security compliance is monitored through:
- Automated security monitoring and alerting
- Internal audits (minimum annually)
- External audits and certifications (ISO 27001, PCI DSS)
- Regulatory examinations (BaFin, ECB)
- Penetration testing and vulnerability assessments
- Access reviews and entitlement audits

---

## 9. Information Security Awareness and Training

### 9.1 Security Awareness Program

EuroTrust Bank AG maintains a comprehensive security awareness program including:

- **Mandatory annual security awareness training** for all employees
- **New employee onboarding** security training
- **Role-based training** for IT, developers, managers, privileged users
- **Phishing simulation exercises** (monthly)
- **Security communications** via email, intranet, posters
- **Lunch-and-learn sessions** on emerging threats
- **Specialized training** for incident responders, security team

### 9.2 Training Objectives

Security training ensures employees can:
- Recognize phishing, social engineering, and cyber threats
- Protect passwords and credentials
- Handle sensitive information appropriately
- Report security incidents promptly
- Understand their security responsibilities
- Make security-conscious decisions

---

## 10. Risk Management

### 10.1 Risk Assessment

Information security risks are assessed systematically and regularly:

- **Annual comprehensive risk assessment** of all in-scope assets and processes
- **Ad-hoc risk assessments** for new projects, systems, or significant changes
- **Methodology:** ISO 27005 risk assessment framework
- **Risk criteria:** Likelihood and impact assessed on 5-point scales
- **Risk owners:** Assigned for all identified risks

### 10.2 Risk Treatment

Risks are treated according to one of the following strategies:
- **Mitigate:** Implement controls to reduce risk to acceptable levels
- **Accept:** Accept residual risk with approval from risk owner and CISO
- **Transfer:** Transfer risk through insurance or outsourcing
- **Avoid:** Eliminate the activity or asset creating the risk

All high and critical risks must have approved treatment plans.

### 10.3 Risk Acceptance

Residual risks are accepted only when:
- Risk is reduced to acceptable levels through controls
- Risk acceptance is documented and approved by risk owner and CISO
- Risk is reviewed regularly (at least annually)

---

## 11. Incident Management

### 11.1 Incident Reporting

All employees must report suspected information security incidents immediately via:
- **Security hotline:** +49-69-SECURITY (24/7)
- **Email:** security-incident@eurotrust-bank.eu
- **Service desk:** IT service management system
- **Direct contact:** CISO or security team member

### 11.2 Incident Classification

Incidents are classified by severity:

| Severity | Definition | Response Time | Notification |
|----------|------------|---------------|--------------|
| **Critical** | Significant data breach, system compromise, major service outage | Immediate | Executive management, Board, regulators |
| **High** | Limited data exposure, security control failure, targeted attack | Within 1 hour | CISO, business unit heads |
| **Medium** | Malware infection, policy violation, minor data loss | Within 4 hours | CISO, IT management |
| **Low** | Suspicious activity, potential vulnerability, minor incident | Within 24 hours | Security team |

### 11.3 Regulatory Reporting

Security incidents meeting regulatory thresholds are reported:
- **GDPR data breaches:** 72 hours to data protection authority
- **BaFin significant incidents:** Without undue delay
- **ECB/SSM cyber incidents:** According to supervisory expectations

---

## 12. Business Continuity and Resilience

EuroTrust Bank AG maintains business continuity and disaster recovery capabilities to ensure:

- **Critical banking services** remain available or are restored within defined timeframes
- **Maximum tolerable period of disruption (MTPD)** is not exceeded
- **Recovery time objectives (RTO)** are met for all critical systems
- **Recovery point objectives (RPO)** limit acceptable data loss
- **Annual BC/DR testing** validates plan effectiveness
- **Crisis management** procedures activate during major incidents

---

## 13. Related Policies and Documents

This Information Security Policy is supported by the following policies, standards, and procedures:

**Policies:**
- ETB-ISMS-POL-002: Acceptable Use Policy
- ETB-ISMS-POL-003: Data Classification and Handling Policy
- ETB-ISMS-POL-004: Access Control Policy
- ETB-ISMS-POL-005: Business Continuity Policy
- ETB-ISMS-POL-006: Incident Response Policy

**Standards:**
- ETB-ISMS-STD-001: Cryptographic Standards
- ETB-ISMS-STD-002: Password and Authentication Standards
- ETB-ISMS-STD-003: Secure Development Standards
- ETB-ISMS-STD-004: Cloud Security Standards

**Procedures:**
- ETB-ISMS-PROC-001: User Access Management Procedure
- ETB-ISMS-PROC-002: Incident Response Procedure
- ETB-ISMS-PROC-003: Change Management Procedure
- ETB-ISMS-PROC-004: Backup and Restoration Procedure
- ETB-ISMS-PROC-005: Vulnerability Management Procedure

**Registers:**
- ETB-ISMS-DOC-004.1: Context of the Organization
- ETB-ISMS-DOC-004.2: Interested Parties Register
- ETB-ISMS-DOC-004.3: ISMS Scope
- ETB-ISMS-DOC-005.31: Legal, Regulatory and Contractual Requirements Register
- ETB-ISMS-DOC-006.1: Risk Assessment and Treatment Methodology
- ETB-ISMS-DOC-006.2: Statement of Applicability

---

## 14. Policy Review and Maintenance

### 14.1 Review Frequency

This Information Security Policy is reviewed:

- **Annually** as part of the management review process
- **When significant changes occur:**
  - Organizational restructuring
  - New regulatory requirements
  - Major security incidents
  - Changes in threat landscape
  - Technology or business model changes
  - Audit findings or recommendations

### 14.2 Policy Approval

All changes to this policy must be:
1. Proposed by the CISO with justification
2. Reviewed by Chief Risk Officer and Chief Compliance Officer
3. Approved by Chief Executive Officer
4. Presented to Board of Directors for notation
5. Communicated to all employees

### 14.3 Version Control

Policy versions are managed with:
- Version numbering (major.minor format)
- Change history documentation
- Approval signatures and dates
- Effective date clearly stated

---

## 15. Communication and Awareness

This Information Security Policy is:

- **Published** on the internal employee portal
- **Communicated** to all employees via email and team meetings
- **Included** in new employee onboarding materials
- **Referenced** in employment contracts and NDAs
- **Available** to external parties (summary version) upon request
- **Reinforced** through regular security awareness communications

---

## 16. Policy Approval

This Information Security Policy has been reviewed and approved by:

| Name | Role | Signature | Date |
|------|------|-----------|------|
| Thomas Müller | Chief Executive Officer | *[Digital Signature]* | 14-Feb-2026 |
| Dr. Stefan Weber | Chief Information Security Officer | *[Digital Signature]* | 14-Feb-2026 |
| Martin Hoffmann | Chief Risk Officer | *[Digital Signature]* | 14-Feb-2026 |
| Claudia Bergmann | Chief Compliance Officer | *[Digital Signature]* | 14-Feb-2026 |

**Board of Directors Acknowledgment:**

This policy has been presented to the Board of Directors of EuroTrust Bank AG on 14 February 2026 and acknowledged as the authoritative direction for information security across the organization.

**Signed:**  
*[Board Chair Digital Signature]*  
**Dr. Wolfgang Schmidt**  
Chairman of the Supervisory Board

---

**END OF DOCUMENT**

*This document is prepared for educational purposes as part of an ISO 27001 audit training scenario. EuroTrust Bank AG is a fictional entity created for learning purposes.*
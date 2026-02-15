# ISO 27001 Risk Register Template

## Document Control
- **Document Version:** 1.0  
- **Last Updated:** 2026-02-15  
- **Author:** [Your Name]  
- **Reviewed By:** [Reviewer Name]  
- **Approval Date:** [Approval Date]  

## Risk Assessment Methodology

### Likelihood Scale (1-5)
1. Rare  
2. Unlikely  
3. Possible  
4. Likely  
5. Almost Certain  

### Impact Scale (1-5)
1. Insignificant  
2. Minor  
3. Moderate  
4. Major  
5. Catastrophic  

### Risk Matrix  
| Likelihood / Impact | 1 (Insignificant) | 2 (Minor) | 3 (Moderate) | 4 (Major) | 5 (Catastrophic) |
|---------------------|-------------------|-----------|---------------|-----------|------------------|
| 1 (Rare)           | Low               | Low       | Low           | Low       | Medium           |
| 2 (Unlikely)       | Low               | Low       | Medium        | Medium    | High             |
| 3 (Possible)       | Low               | Medium    | Medium        | High      | Critical         |
| 4 (Likely)         | Medium            | Medium    | High          | High      | Critical         |
| 5 (Almost Certain) | Medium            | High      | High          | Critical  | Critical         |

## Sample Risk Entries
| Risk ID | Asset                       | Asset Classification | Vulnerability                | Threat               | Threat Actor                        | Impact Category    | Inherent Likelihood | Inherent Impact | Inherent Risk Score | Inherent Risk Level | Existing Controls | Residual Likelihood | Residual Impact | Residual Risk Score | Residual Risk Level | Risk Treatment | Treatment Controls/Actions | Control Owner  | Risk Owner | Target Completion Date | Review Date | Status |
|---------|-----------------------------|----------------------|-----------------------------|----------------------|-------------------------------------|---------------------|----------------------|------------------|----------------------|----------------------|------------------|----------------------|------------------|---------------------|----------------------|----------------|---------------------------|----------------|------------|-------------------------|-------------|--------|
| 1       | Customer Database           | Sensitive            | SQL Injection               | Unauthorized Access   | Cyber Criminals                    | Confidentiality     | 4                    | 5                | 20                   | Critical             | Firewall          | 3                    | 4                | 12                   | High                 | Mitigate       | Implement WAF            | IT Security    | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 2       | Ransomware Protection       | Critical             | Absence of Backups          | Data Encryption      | Cyber Criminals                    | Availability        | 5                    | 5                | 25                   | Critical             | Antivirus         | 4                    | 4                | 16                   | High                 | Mitigate       | Regular Backups         | IT Operations  | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 3       | Insider Threat Monitoring    | Sensitive            | Lack of Awareness Training  | Data Theft           | Insider Employee                    | Confidentiality     | 4                    | 5                | 20                   | Critical             | Monitoring        | 2                    | 4                | 8                    | Medium               | Mitigate       | Employee Training       | HR             | CISO       | 2026-06-30              | 2026-05-31  | Open   |
| 4       | Cloud Data Storage          | Critical             | Unsecured APIs             | Data Breach          | Cyber Criminals                    | Confidentiality     | 4                    | 4                | 16                   | High                 | Encryption        | 3                    | 4                | 12                   | High                 | Mitigate       | Secure APIs            | IT Security    | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 5       | SWIFT Transaction System    | Critical             | Human Error                | Financial Fraud      | Cyber Criminals                    | Availability        | 3                    | 5                | 15                   | High                 | Monitoring        | 2                    | 4                | 8                    | Medium               | Mitigate       | Dual Control System     | Finance Dept   | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 6       | Physical Security Measures   | Critical             | Improper Access Control     | Theft                | Insider/Outsider                   | Availability        | 3                    | 5                | 15                   | High                 | Security Guards   | 2                    | 3                | 6                    | Medium               | Mitigate       | Access Control Review   | Facilities      | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 7       | Mobile Application          | Sensitive            | Lack of Testing            | Application Breach    | Cyber Criminals                    | Confidentiality     | 4                    | 4                | 16                   | High                 | Secure Coding     | 3                    | 4                | 12                   | High                 | Mitigate       | Conduct Pen Tests      | IT Security    | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 8       | GDPR Compliance             | Regulatory           | Lack of Policies           | Fines                | Regulatory Body                    | Legal               | 5                    | 5                | 25                   | Critical             | Training          | 4                    | 3                | 12                   | High                 | Mitigate       | Policy Implementation    | Legal Dept     | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 9       | Business Continuity Plans   | Critical             | Poor Documentation          | Operational Failure   | Management                          | Availability        | 4                    | 5                | 20                   | Critical             | Backup Systems    | 3                    | 4                | 12                   | High                 | Mitigate       | BCP Training            | Management      | CISO       | 2026-12-31              | 2026-11-30  | Open   |
| 10      | Supply Chain Verification    | Critical             | Weak Vendor Assessment      | Data Breach          | Third-party Vendor                  | Integrity           | 4                    | 5                | 20                   | Critical             | Vendor Contracts   | 2                    | 4                | 8                    | Medium               | Mitigate       | Regular Assessments    | Procurement     | CISO       | 2026-12-31              | 2026-11-30  | Open   |

## Risk Summary Dashboard
- **Total Risks:** 10  
- **Critical Risks:** 5  
- **High Risks:** 5  
- **Medium Risks:** 3  
- **Low Risks:** 0  

## Instructions for Excel Format
- **Columns:**  
  - Risk ID  
  - Asset  
  - Asset Classification  
  - Vulnerability  
  - Threat  
  - Threat Actor  
  - Impact Category  
  - Inherent Likelihood  
  - Inherent Impact  
  - Inherent Risk Score  
  - Inherent Risk Level  
  - Existing Controls  
  - Residual Likelihood  
  - Residual Impact  
  - Residual Risk Score  
  - Residual Risk Level  
  - Risk Treatment  
  - Treatment Controls/Actions  
  - Control Owner  
  - Risk Owner  
  - Target Completion Date  
  - Review Date  
  - Status  

This document serves as a comprehensive template for implementing an ISO 27001 risk register in your organization. Customize it according to your specific needs and assessments.
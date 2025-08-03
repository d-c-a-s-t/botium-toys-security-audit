# botium-toys-security-audit
# Internal Security Audit – Botium Toys

Overview
An internal audit conducted as part of a cybersecurity training course. The goal was to assess Botium Toys’ security controls and compliance posture using the NIST CSF framework.

 Audit Scope and Goals
- **Scope:** Entire security program, including digital and physical assets
- **Goals:** Assess existing controls and compliance gaps to improve security posture

 Risk Assessment Summary
- High-level risk score (8/10)
- No access controls or encryption for customer credit card data
- Weak password policies and no IDS
- Backups and disaster recovery plans missing
- Employees have access to customer PII/SPII

 Controls Assessment Results

| Control                         | Control Name / Type      | In Place? | Notes                                             
|---------------------------------|--------------------------|-----------|---------------------------------------------------------------------|
| Least Privilege                 | Admin / Preventative     | No        | Not implemented. All employees have access to sensitive information |
| Disaster Recovery Plan          | Admin / Corrective       | No        | No documented recovery plan or backups in place                     |
| Password Policies               | Admin / Preventative     | No        | Password policy exists but lacks complexity and enforcement         |
| Separation of Duties            | Admin / Preventative     | No        | Not implemented; No role-based controls separation                  |
| Firewall                        | Technical / Preventative | Yes       | In place and configured with security rules                         |
| Intrusion Detection System (IDS)| Technical / Preventative | No        | IDS not installed; network threats may go undetected                |
| Backups                         | Technical / Corrective   | No 	 | No backups in place; data recovery not possible in a loss event     |
| Antivirus Software              | Technical / Corrective   | Yes       | Installed and regularly monitored by IT department                  |
| Legacy Systems                  | Technical / Preventative | No        | Monitoring exists but lacks schedule and clear intervention process |
| Encryption                      | Technical / Deterrent    | No        | Not in use; customer credit card data is unprotected                |
| Password Management System      | Technical / Preventative | No        | Not centralized system; enforcement and resets are inconsistent     | 
| Locks (office/store/warehouse   | Physical / Preventative  | Yes       | Physical locations are secured with adequate locks                  | 
| Closed-Circuit TV Surveillance  | Physical / Preventative  | Yes       | CCTV is up to date and used to monitor physical premises            |
| Fire Detection/Prevention System| Physical / Detective     | Yes       | Fire alarm and prevention systems are in place and functioning      | 


 Compliance Assessment – PCI DSS

| Best Practice                                                           | In Place? | Notes                                                                                                        |
|-------------------------------------------------------------------------|-----------|--------------------------------------------------------------------------------------------------------------|
| Only authorized users have access to customers’ credit card info.       | No        | All employees have access; access controls not yet implemented.                                              |
| Credit card info is stored, accepted, processed, in secured environments| No        | No encryption is in place; credit card data is stored in plaintext                                           |
| Data encryption procedures implemented to better secure credit card     | No        | No encryption in in place; data is exposed at multiple points                                                | 
| Adopt secure password management policies                               | No        | Password policy exists but lacks standard complexity requirements & Not enforced by central management system|
 

 Compliance Assessment – General Data Protection Regulation (GDPR)

| Best Practice                                                           | In Place? | Notes                                                                                        |
|-------------------------------------------------------------------------|-----------|----------------------------------------------------------------------------------------------|
| E.U. Customer's data is kept private/secured                            | No        | Encryption currently not used; credit card is unprotected                                    |
| There is a plan to notify E.U. Customer within 72hrs if data breach     | Yes       | Notification plan in place; supported by enforced privacy policies and procedures            |
| Ensure data is properly classified and inventoried                      | No        | No clear indication that data is properly classified or inventoried to meet GDPR standards   |
| Enforce privacy policies, procedures, and processes properly doc data   | Yes       | Privacy policies and procedures are developed, enforced, and maintained                      | 



 Compliance Assessment – System and Organizations Controls (SOC type 1, SOC type 2)

| Best Practice                                                              | In Place? | Notes                                                                                               |
|----------------------------------------------------------------------------|-----------|-----------------------------------------------------------------------------------------------------|
| User access policies are established                                       | No        | User access policies not established; allowing all employees unrestricted access including PII/SPII |                                 | Sensitive data (PII/SPII) is confidential/private                          | No        | Sensitive data is not kept confidential; all employees have access to stored internal data          |
| Data integrity ensures data is consistent, complete, accurate and validated| Yes       | IT has implemented integrated controls to ensure data integrity, consistency, and validation        |
| Data is available to individuals authorized to access it                   | No        | All employees have unrestricted access to sensitive data; violating authorization standards         | 





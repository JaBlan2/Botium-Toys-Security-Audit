# Botium Toys Security Audit

## Introduction
This is an internal security audit done as a practice to hone my skills and give me experience in doing security audits. This audit is performed on the fictitious company Barium Toys, and was completed as a part of my Cybersecurity Portfolio alongside Google's [Cybersecurity Professional Certificate](https://www.coursera.org/google-certificates/cybersecurity-certificate) on Coursera. This is course 2, [Play It Safe: Manage Security Risks](https://www.coursera.org/learn/manage-security-risks?specialization=google-cybersecurity).

The goal of this audit is to find security flaws in Botium Toys' cybersecurity program. This includes their assets (such as employee equipment and devices), their internal network, and their systems. I will be using a controls and compliance checklist to determine best practices that need to be implemented to improve their security posture.

## Scenario
Botium Toys is a small U.S. business that develops and sells toys. They have a single physical location that houses most of the operations besides manufacturing. Recently, Botium Toys' online presence has grown, attracting customers outside of the U.S. such as in the European Union. As a result, their information technology department is under pressure to support their market worldwide.

Their IT department's manager has decided that they should perform an internal IT audit, as she is worried about maintaining compliance and business operations as the company continues to grow without clear guidelines. She believes that an internal audit will help to secure the company's infrastructure and help them identify and mitigate potential risks, vulnerabilities, or threats to assets. The manager is also interested in ensuring that they comply with regulations for conducting business in the European Union and internally processing and accepting online payments.

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing IT assets, and completing a risk assessment, with the goal to provide an overview of risks or fines that the company might experience due to the current state of their security posture.

I will review the IT manager's scope, goals, and risk assessment report and then perform an internal audit by completing a controls and compliance checklist.



## Scope, Goals, and Risk Assessment Report

### Scope
The scope of this audit is defined as the entire security program at Botium Toys. This includes their assets like employee equipment and devices, their internal network, and their systems. You will need to review the assets Botium Toys has and the controls and compliance practices they have in place.

### Goals
Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices that need to be implemented to  improve Botium Toys’ security posture.

### Current IT Assets
  * On-premises equipment for in-office business needs  
  * Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
  * Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
  * Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
  * Internet access
  * Internal network
  * Data retention and storage
  * Legacy system maintenance: end-of-life systems that require human monitoring 

### Risk Assessment

#### Risk Description
Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards.

#### Control Best Practices
The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

#### Risk Score
On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

#### Additional Comments
The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:
  * Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.
  * Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database. 
  * Access controls pertaining to least privilege and separation of duties have not been implemented.
  * The IT department has ensured availability and integrated controls to ensure data integrity.
  * The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
  * Antivirus software is installed and monitored regularly by the IT department. 
  * The IT department has not installed an intrusion detection system (IDS).
  * There are no disaster recovery plans currently in place, and the company does not have backups of critical data. 
  * The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
  * Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters). 
  * There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
  * While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
  * The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.

## Controls and Compliance Assessment

### Controls Assessment

#### Administrative/Managerial Controls
| Control Name | Needs to be Implemented (X) | Explanation |
|---|:---:|---|
|Least Privilege|X|All employees currently have access to customer data. This should be limited to reduce the risk of a data breach|
|Disaster Recovery Plans|X|No disaster recovery is in place. It should be implemented to ensure business continuity|
|Password Policies|X|Current password policies are weak and cause problems. This could lead to a data breach of data|
|Separation of Duties|X|Needs to be implemented to reduce fraudulent access to critical data|



#### Technical Controls
| Control Name | Needs to be Implemented (X) | Explanation |
|---|:---:|---|
| Firewall | |Firewall is currently active and maintained|
| Intrusion Detection System (IDS)| X | Needs to be implemented to help reduce the damage of an intruder|
| Backups |X | Needs to be implemented to restore/recover in the event of an attack|
| Antivirus Software|  | Antivirus is currently active and maintained|
| Manual Monitoring, Maintenance, and Intervention for Legacy Systems| X | A regular schedule should be implemented to reduce the possibility of a risk | 
| Encryption |X| Should be implemented to improve PII/SPII security|
| Password Management | X | There is currently no password management in place. Implementing would improve against password fatigue|



#### Physical/Operational Controls
| Control Name | Needs to be Implemented (X) | Explanation |
|---|:---:|---|
| Locks (offices, storefront, warehouse) | | Locks have been installed|
| Closed-circuit television (CCTV) surveillance|| CCTV has been installed|
| Fire detection/prevention (fire alarm, sprinkler system, etc.) | | Fire detection/prevention has been installed|




### Compliance Assessment

#### Payment Card Industry Data Security Standard (PCI DSS)
| Best Practice | Needs to be Implemented (X) | 
|---|:---:|
|Only authorized users have access to customers’ credit card information| X |
|Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment| X |
|Implement data encryption procedures to better secure credit card transaction touchpoints and data | X |
|Adopt secure password management policies | X |



#### General Data Protection Regulation (GDPR)
| Best Practice | Needs to be Implemented (X) |
|---|:---:|
|E.U. customers’ data is kept private/secured | X|
|There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach||
|Ensure data is properly classified and inventoried|X|
|Enforce privacy policies, procedures, and processes to properly document and maintain data||



#### System and Organizations Controls (SOC type 1, SOC type 2)
| Best Practice | Needs to be Implemented (X) |
|---|:---:|
|User access policies are established|X|
|Sensitive data (PII/SPII) is confidential/private|X|
|Data integrity ensures the data is consistent, complete, accurate, and has been validated||
|Data is available to individuals authorized to access it|X|



### Recommendations
Upon assessment, we need to update many controls in order to prevent risk and prepare for international business. I would emphasize the need to secure our data internally, then we can look into expanding business. Our customers' data should be a top priority as well, and we are currently not encrypting most of their data. I would suggest the plan of action being the following, based on risk posed, to improve our security posture:
1. Secure customer data (encryption)
2. Implement intrusion detection systems and data backups
3. Secure office accounts (password policies, separation of duties, etc)
4. Address any outliers in the assessment above

Doing this should also help Botium Toys to begin complying with E.U. and U.S. regulations, allowing for less risk of fines in the future. Botium Toys should also properly classify assets in order to identify any other controls that may need to be implemented.



## Conclusion
After completing this activity and reviewing my response, I see that I did well in assessing what has and has not been implemented already. I was able to accurately identify what Botium Toys needs to implement in order to reach compliance and what should be done to secure their data. I can improve on my ability to rank these issues based on risk however, as I struggled to figure out which aspects were more important to be completed sooner rather than later.


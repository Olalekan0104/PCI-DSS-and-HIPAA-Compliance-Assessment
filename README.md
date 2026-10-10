MediCare Plus Hospital: PCI DSS and HIPAA Compliance Assessment
This project assesses PCI DSS and HIPAA compliance gaps at MediCare Plus Hospital, focusing on payment card security and the protection of patient health information. It identifies relevant security requirements, evaluates access control weaknesses, and recommends practical remediation measures to strengthen compliance and reduce risk.
Table of Contents
- Project Overview
- Network Topology
- Tools and Technologies
- Configuration Steps
- Results and Findings
- Author
Project Overview
MediCare Plus Hospital accepts card payments at its reception desk and through an online patient portal. It also maintains an Electronic Health Record (EHR) system containing patient health information.
The assessment examines two scenarios:
- Incident 1: PCI DSS Compliance. Cardholder data is transmitted to a third-party payment processor, requiring an assessment of payment security, data transmission, access controls, and the scope of applicable PCI DSS requirements.
- Incident 2: HIPAA Compliance. Several employees can access patient records without a job-related need, creating potential privacy and security risks.
The main objectives are to:
- Identify applicable PCI DSS requirements and HIPAA safeguards.
- Identify compliance gaps and weaknesses in existing security practices.
- Recommend preventive, detective, and corrective security measures.
- Strengthen access management and protection of sensitive information.
- Develop practical remediation recommendations and identify evidence needed to validate control effectiveness.
This is a scenario-based assessment. The findings are recommendations based on the supplied project information, not a formal compliance certification or confirmation that controls have been implemented.
Network Topology
The project describes a logical view of the hospital's payment processing and patient information environment. It does not provide specific IP addresses, subnet configurations, network devices, or a physical network diagram.
Logical Environment
                  MediCare Plus Hospital
                            |
             +--------------+--------------+
             |                             |
       Payment Systems                Clinical Systems
             |                             |
     +-------+--------+                    |
     |                |                    |
 Reception Desk   Online Portal           EHR System
     |                |                    |
     +-------+--------+                    |
             |                             |
      Payment Processor              Patient Records
             |                             |
      Cardholder Data                Electronic PHI
             |                             |
       PCI DSS Controls              HIPAA Safeguards
             |                             |
      Encryption and                 Access Control
      Access Security                Audit Controls


Key Components
- Reception Payment System: Accepts payment cards for medical bills.
- Online Patient Portal: Provides an online channel for payment processing.
- Payment Processor: Receives cardholder data transmitted by the hospital.
- Electronic Health Record (EHR) System: Stores and manages patient records and electronic protected health information (ePHI).
- Access Control Mechanisms: Restrict access to authorized personnel according to job responsibilities.
- Audit and Monitoring Controls: Support the detection and investigation of inappropriate access and suspicious activity.
The actual PCI DSS scope must be confirmed using the hospital's payment data flows and system architecture. The available scenario does not establish whether the hospital itself stores cardholder data.
Tools and Technologies
- PCI DSS: Payment Card Industry Data Security Standard for protecting payment account data.
- HIPAA Security Rule: Requirements for protecting electronic protected health information.
- Electronic Health Record (EHR): System used to manage patient records.
- Role-Based Access Control (RBAC): Restricts access according to assigned organizational roles.
- Least Privilege: Limits user permissions to what is necessary for assigned duties.
- Encryption: Protects cardholder data during transmission where required.
- Audit Logging and Monitoring: Records and supports review of activity involving sensitive information.
- Microsoft PowerPoint: Used in preparing the original assignment presentation.
- PDF: Used to document and present the completed compliance assessment.
- GitHub: Used to maintain and showcase the project as part of a GRC portfolio.
No specific vulnerability scanners, SIEM platforms, firewall products, or network configuration tools were identified in the original scenario.
Configuration Steps
1. Review the business environment. Examined the hospital's payment processing activities, EHR system, patient information, and third-party payment relationship.
2. Identify applicable compliance requirements. Reviewed PCI DSS requirement areas relevant to payment processing and HIPAA safeguards relevant to electronic patient records.
3. Assess the payment security scenario. Identified the need to confirm PCI DSS scope, document payment data flows, validate secure transmission, and determine whether cardholder data is stored.
4. Assess the patient record scenario. Identified excessive employee access as a potential compliance gap requiring investigation and remediation.
5. Identify relevant HIPAA safeguards. Considered technical safeguards, including access controls and audit controls, alongside administrative safeguards governing access authorization and security management.
6. Identify compliance gaps. Documented potential weaknesses in payment security, access restrictions, monitoring, and supporting policies and procedures.
7. Recommend security controls. Proposed encryption validation, role-based access, least privilege, unique user accounts, audit-log reviews, and documented access approval procedures.
8. Develop a remediation plan. Identified suggested priorities, responsible teams, and evidence that could demonstrate whether corrective actions were completed.
9. Document the assessment. Consolidated the analysis, recommendations, limitations, and references into a professional PDF report for portfolio use.
Results and Findings
The assessment identified two primary areas requiring attention.
PCI DSS Findings
- Cardholder data is transmitted to an external payment processor, making secure transmission and payment data flow assessment important.
- The hospital's PCI DSS scope needs to be established based on the systems and services involved in payment processing.
- Whether cardholder data is stored by the hospital remains unconfirmed and requires investigation.
- Access controls, logging, monitoring, and other applicable security requirements should be reviewed against the confirmed scope.
Recommended actions: Document payment data flows, validate encryption and secure transmission, minimize cardholder data storage, restrict access to payment systems, and track identified compliance gaps through remediation.
HIPAA Findings
- Several employees can access patient records without a demonstrated job-related need.
- Excessive permissions increase the risk of inappropriate access or disclosure of patient information.
- Audit controls are important for determining who accessed records and supporting investigations.
- Administrative policies and procedures should govern access approval, role changes, and periodic access reviews.
Recommended actions: Review and remove unnecessary permissions, apply least privilege, use unique user accounts, review access logs, establish documented access approval procedures, and provide appropriate workforce training.
Overall Outcome
The project demonstrates how a GRC Analyst can connect compliance requirements to business risks, identify potential control gaps, recommend corrective actions, and define evidence needed to validate remediation.
The assessment provides a foundation for a more secure payment environment and better protection of patient information. Actual compliance status and control effectiveness would need to be verified through further evidence collection and testing.
Author
- Project: MediCare Plus Hospital PCI DSS and HIPAA Compliance Assessment
- Specialization: Governance, Risk, and Compliance (GRC)
- Focus Areas: Regulatory Compliance, Security Controls, Access Management, and Risk Remediation
- LinkedIn: linkedin.com/in/saheed-i-0008b11bb

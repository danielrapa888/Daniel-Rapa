# Botium Toys Security Audit Report

The following security audit is an activity which forms part of the Google Cybersecurity Certificate. 

## 1. Scope and Objectives

### Scope
The scope of this audit covers the entire security program of Botium Toys, including all physical and digital assets, IT systems, internal processes, and compliance with relevant security regulations such as PCI DSS, GDPR, and SOC 1/2.

### Objectives
- Assess existing controls and compliance posture.  
- Identify gaps in controls and regulatory adherence.  
- Provide recommendations to strengthen Botium Toys’ overall security framework.

---

## 2. Current Assets

The following assets are managed by the IT Department and are included within the audit scope:

- On-premises office and retail equipment.  
- Employee end-user devices (desktops, laptops, smartphones, peripherals).  
- Internal and external networks, including e-commerce and database systems.  
- Customer data storage and payment processing systems.  
- Warehouse and storefront facilities (CCTV, locks, fire detection systems).  
- Legacy systems requiring manual oversight and maintenance.

---

## 3. Risk Assessment Summary

| **Category** | **Details** |
|---------------|-------------|
| **Risk Description** | Inadequate asset management, insufficient controls, and incomplete regulatory compliance. |
| **Risk Score** | 8 / 10 (High) |
| **Impact** | Medium to High — potential for data breach, loss of compliance, or operational downtime. |
| **Key Risk Drivers** | - Lack of encryption for customer and payment data.<br>- Universal access to internal data.<br>- Absence of disaster recovery and backup plans.<br>- Weak password policies and lack of password manager.<br>- No intrusion detection system (IDS).<br>- Irregular legacy system monitoring. |

---

## 4. Controls Assessment

| **Control** | **Implemented** | **Category** | **Control Type** | **Risk if Missing** |
|--------------|----------------|---------------|------------------|--------------------|
| Least Privilege | No | Administrative | Preventative | Unauthorized access and data exposure |
| Separation of Duties | No | Administrative | Preventative | Insider threats or lack of accountability |
| Password Policy | Partial | Administrative | Preventative | Increased vulnerability to brute-force attacks |
| Password Management System | No | Technical | Preventative | Weak password hygiene and inefficient recovery |
| Firewall | Yes | Technical | Preventative | Network intrusion risk |
| Intrusion Detection System (IDS) | No | Technical | Detective | Failure to detect or respond to anomalies |
| Antivirus Software | Yes | Technical | Corrective | Threat detection and containment gap |
| Encryption | No | Technical | Deterrent | Breach of confidentiality for PII and payment data |
| Backups | No | Technical | Corrective | Irrecoverable data loss |
| Disaster Recovery Plan | No | Administrative | Corrective | Business continuity failure |
| Legacy Systems Monitoring | Partial | Technical | Preventative | Undetected vulnerabilities and outdated systems |
| Locks / CCTV / Fire Systems | Yes | Physical | Preventative / Detective | Physical theft or damage |

---

## 5. Compliance Audit

### 5.1 PCI DSS (Payment Card Industry Data Security Standard)

| **Requirement** | **Compliant** | **Notes** |
|------------------|----------------|-----------|
| Restrict access to cardholder data | No | All employees currently have access. |
| Secure transmission and storage of cardholder data | No | Encryption not implemented. |
| Data encryption at all touchpoints | No | Not in place. |
| Secure password management | No | Weak policy; no centralized enforcement. |

**Risk:** Noncompliance may result in significant fines and loss of payment processing privileges.

---

### 5.2 GDPR (General Data Protection Regulation)

| **Requirement** | **Compliant** | **Notes** |
|------------------|----------------|-----------|
| Data privacy and protection | No | Data unencrypted and widely accessible. |
| 72-hour breach notification plan | Yes | Plan established by the IT Department. |
| Data classification and inventory | No | Assets not fully inventoried or categorized. |
| Privacy policies and documentation | Yes | Policies exist but are not consistently enforced. |

**Risk:** Potential exposure to EU penalties and reputational harm.

---

### 5.3 SOC 1 / SOC 2 (System and Organization Controls)

| **Requirement** | **Compliant** | **Notes** |
|------------------|----------------|-----------|
| User access policies | No | Lack of role-based access control. |
| Confidentiality of sensitive data (PII/SPII) | No | Weak protection mechanisms. |
| Data integrity controls | Yes | Maintained through firewalls and antivirus software. |
| Data availability | Yes | Systems operational, but lack of redundancy. |

**Risk:** Limited assurance to stakeholders and incomplete compliance posture.

---

## 6. Recommendations

### High Priority (Immediate Action)
1. **Implement Data Encryption** for all customer, payment, and sensitive business data.  
2. **Deploy an Intrusion Detection System (IDS)** to monitor and alert on anomalous traffic.  
3. **Establish Least Privilege and Separation of Duties Policies** to restrict access based on role and responsibility.  
4. **Develop a Disaster Recovery and Backup Plan** to ensure data continuity and resilience.  
5. **Adopt a Centralized Password Management System** to enforce strong password policies and self-service recovery.

### Medium Priority
- Schedule regular monitoring and maintenance for legacy systems.  
- Conduct a complete inventory and classification of all assets.  
- Expand organization-wide data privacy and security awareness training.

### Low Priority
- Periodically test physical security systems (locks, CCTV, fire suppression).  
- Perform quarterly internal security audits.

---

## 7. Conclusion

The security audit of Botium Toys indicates significant gaps in administrative and technical controls. The organization’s current risk posture is high, primarily due to insufficient data protection mechanisms, lack of access control policies, and absence of recovery planning.  

By implementing the recommended measures—particularly encryption, access management, and business continuity planning—Botium Toys can substantially improve its compliance alignment, reduce data breach risk, and strengthen overall cybersecurity resilience.

---

**Prepared by:** [Your Name]  
**Date:** [Insert Date]  
**Project:** Coursera — Manage Security Risks Portfolio Activity  

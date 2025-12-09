---
title: "Event 5"
date: 2025-11-29
weight: 5
chapter: false
pre: "<b> 4.5. </b>"
---

# Workshop Report: Cloud Security Based on AWS Well-Architected Framework

## 1. Participation Goals
With cybersecurity threats becoming increasingly sophisticated, this workshop provided a crucial opportunity to strengthen my understanding of the **Security Pillar**. My objectives included:
- Embracing modern security principles: **Zero Trust**, **Least Privilege**, and **Defense in Depth**.
- Gaining proficiency in 5 critical security domains: Identity Management (IAM), Threat Detection, Infrastructure Protection, Data Protection, and Incident Response.
- Learning practical insights from industry experts to identify and defend against common attack scenarios in the Vietnamese market.

## 2. Event Details
- **Date & Time:** 08:30 – 12:00 | Saturday, November 29, 2025.
- **Venue:** 26th Floor, Bitexco Financial Tower, District 1, Ho Chi Minh City.
- **Speakers:** AWS Cloud Club Captains, AWS Community Builders, and special guest **Mendel Grabski** (Cloud Security Architect).

## 3. Core Knowledge

### Identity & Access Management (IAM)
- **Identity is the New Firewall:** In cloud-native environments, identity management has become more critical than traditional network firewalls.
- **Zero Trust Architecture:** Eliminating the "trust internal network" mindset. Every access request must undergo strict authentication.
- **Authentication Modernization:** Eliminating long-term Access Keys in favor of **IAM Roles** and **Identity Center (SSO)**. Leveraging **Access Analyzer** to audit and remove excessive permissions.

### Threat Detection & Infrastructure Protection
- **Centralized Visibility:** Using **AWS Security Hub** as the command center, aggregating alerts from GuardDuty, Inspector, and Macie.
- **Defense in Depth:** Establishing multiple protection layers from Network (VPC, Security Groups) to Edge (WAF, Shield).
- **Encryption Everywhere:** Encryption is mandatory. Using KMS for data at rest and TLS 1.2+ for data in transit.

### Automated Incident Response (IR)
- **IR Lifecycle:** Standardizing the process: Preparation → Detection → Containment → Recovery.
- **Automation:** Instead of slow manual handling, using **Lambda** and **Step Functions** for automated responses (e.g., automatically revoking IAM permissions upon detecting anomalous behavior).

## 4. Insights & Lessons Learned
- **Security by Design:** Security is not an add-on feature; it must be integrated from the very first line of code.
- **Assume Breach Mentality:** Always design systems assuming "we have already been compromised." This focuses efforts on minimizing the Blast Radius and optimizing recovery speed.
- **Immutable Infrastructure:** Minimizing SSH access to servers for troubleshooting; instead, replacing them with new, patched "clean" instances.

## 5. Action Plan
Immediately applying the knowledge gained to strengthen security for the **Serverless Student Management** project:
1.  **IAM Refactoring:** Auditing all policies, removing `*:*` permissions and hardcoded credentials. Transitioning to IAM Roles for Lambda functions.
2.  **Secrets Management:** Migrating all Database Passwords and API Keys from local `.env` configuration files to **AWS Systems Manager Parameter Store** for centralized and secure management.
3.  **Security Monitoring:** Enabling **Amazon GuardDuty** (utilizing Free Tier) for early detection of suspicious activities (such as unauthorized crypto mining on internship accounts).
4.  **Data Protection:** Enabling default Server-Side Encryption (SSE-S3) for all S3 Buckets containing student records.

## 6. Event Experience
The event delivered practical and urgent perspectives on cloud security. The demos on **IAM Policy Validation** and **Automated Incident Response** clearly demonstrated the power of automation in security. Particularly, discussions about real-world use cases in Vietnam deepened my awareness of the responsibility to protect user authentication information.

![All members participated](/images/4-EventParticipated/4.5-Event5/Image_5.2)
![Identity & Access Management](/images/4-EventParticipated/4.5-Event5/Image_5.1)
![The Badging Journey](/images/4-EventParticipated/4.5-Event5/Image_5.3)
![Multi Layer Security against Attack Vectors](/images/4-EventParticipated/4.5-Event5/Image_5.4)
![Special Guest](/images/4-EventParticipated/4.5-Event5/Image_5.5)

> **Summary:** This event transformed my mindset from "build to make it work" to "build securely and sustainably." This is an essential preparation step before deploying any application to a Production environment.

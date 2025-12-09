---
title: "Week 12 Worklog"
date: 2025-11-23
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:

- Setup Security services (WAF, GuardDuty)
- Implement CI/CD Pipeline
- Join AWS Cloud Mastery Series #3 (Security)
- Setup CloudFront and Route53

### Tasks to Execute This Week:

| **Date**          | **Task**                                                                                                                                                                                                                                                                                                       | **Start**  | **Finish** | **References**                     |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ---------------------------------- |
| Monday (24/11)    | - **Setup WAF (Web Application Firewall):**<br>&emsp;+ Create WAF Web ACL<br>&emsp;+ Add AWS Managed Rules:<br>&emsp;&emsp;_ Core Rule Set<br>&emsp;&emsp;_ Known Bad Inputs<br>&emsp;&emsp;\_ SQL Injection Protection<br>&emsp;+ Configure rate limiting (2000 req/5min)<br>- Associate WAF with API Gateway | 24/11/2025 | 24/11/2025 | WAF Documentation                  |
| Tuesday (25/11)   | - **Enable GuardDuty:**<br>&emsp;+ Activate GuardDuty<br>&emsp;+ Review findings<br>&emsp;+ Setup GuardDuty notifications<br>- **Enable Security Hub:**<br>&emsp;+ Centralized security view<br>&emsp;+ Enable security standards                                                                              | 25/11/2025 | 25/11/2025 | GuardDuty Docs / Security Hub Docs |
| Wednesday (26/11) | - **Setup S3 Bucket for Artifacts:**<br>&emsp;+ Create bucket with versioning<br>&emsp;+ Configure lifecycle policies<br>- **Create CodeBuild Project:**<br>&emsp;+ Source: GitLab/GitHub<br>&emsp;+ Environment: Java 17<br>&emsp;+ Buildspec for backend<br>&emsp;+ Test build                               | 26/11/2025 | 26/11/2025 | CodeBuild Guide                    |
| Thursday (27/11)  | - **Create CodePipeline:**<br>&emsp;+ Source stage: GitLab webhook<br>&emsp;+ Build stage: CodeBuild<br>&emsp;+ Deploy stage: Lambda update<br>- Test automated deployment flow<br>- Document CI/CD pipeline                                                                                                   | 27/11/2025 | 27/11/2025 | CodePipeline Docs                  |
| Friday (28/11)    | - **Setup CloudFront Distribution:**<br>&emsp;+ Origin: API Gateway<br>&emsp;+ Configure caching behaviors<br>&emsp;+ HTTPS only<br>&emsp;+ Associate WAF Web ACL<br>- Test CDN performance<br>- Measure latency improvements                                                                                  | 28/11/2025 | 28/11/2025 | CloudFront Guide                   |

### Week 12 Achievements:

- Implemented WAF, GuardDuty, Security Hub — enhanced security and compliance
- Built automated CI/CD pipeline with zero-downtime deployments
- Global distribution via CloudFront improves latency and performance
- Gained security best practices from AWS workshop
- Architecture reaches production-level standards with full security checklist

---

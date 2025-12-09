---
title: "Week 10 Worklog"
date: 2025-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

- Complete Backend APIs for core features
- Deploy Lambda and API Gateway
- Join AWS Cloud Mastery Series #1
- Setup CloudWatch monitoring

### Tasks to Execute This Week:

| **Date**          | **Task**                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | **Start**  | **Finish** | **References** |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | -------------- |
| Monday (10/11)    | - **Implement User Management APIs:**<br>&emsp;+ GET /users<br>&emsp;+ GET /users/{id}<br>&emsp;+ POST /users<br>&emsp;+ PUT /users/{id}<br>&emsp;+ DELETE /users/{id}<br>- Test CRUD operations<br>- Write Week 9 report<br>- **Implement Class Management APIs:**<br>&emsp;+ GET /classes<br>&emsp;+ GET /classes/{id}<br>&emsp;+ POST /classes<br>&emsp;+ PUT /classes/{id}<br>&emsp;+ DELETE /classes/{id}<br>&emsp;+ GET /classes/{id}/students<br>- Test with DynamoDB | 10/11/2025 | 10/11/2025 | -              |
| Tuesday (11/11)   | - **Implement Subject Management APIs:**<br>&emsp;+ GET /subjects<br>&emsp;+ GET /subjects/{id}<br>&emsp;+ POST /subjects<br>&emsp;+ PUT /subjects/{id}<br>&emsp;+ DELETE /subjects/{id}<br>- Implement business logic and validation                                                                                                                                                                                                                                        | 11/11/2025 | 11/11/2025 | -              |
| Wednesday (12/11) | - **Build and Package Lambda:**<br>&emsp;+ Configure pom.xml with maven-shade-plugin<br>&emsp;+ Build JAR: `mvn clean package`<br>&emsp;+ Test locally if possible<br>&emsp;+ Verify JAR size (< 50MB recommended)                                                                                                                                                                                                                                                           | 12/11/2025 | 12/11/2025 | -              |
| Thursday (13/11)  | - **Deploy Lambda Function:**<br>&emsp;+ Create Lambda function in AWS Console<br>&emsp;+ Upload JAR file<br>&emsp;+ Configure Handler, Memory (1024MB), Timeout (30s)<br>&emsp;+ Setup IAM Role with DynamoDB permissions<br>&emsp;+ Test Lambda with sample events                                                                                                                                                                                                         | 13/11/2025 | 13/11/2025 | -              |
| Friday (14/11)    | - **Create API Gateway:**<br>&emsp;+ Create HTTP API or REST API<br>&emsp;+ Configure route: `ANY /{proxy+}`<br>&emsp;+ Enable CORS<br>&emsp;+ Deploy stage: prod<br>&emsp;+ Test endpoints<br>- Document API Gateway URL                                                                                                                                                                                                                                                    | 14/11/2025 | 14/11/2025 | -              |

### Week 10 Achievements:

- Backend APIs (Classes, Subjects) completed and running stably
- Lambda + API Gateway deployed and ready for frontend integration
- Logging and monitoring with CloudWatch configured
- Participated in AWS workshop, researched AI/ML for future features
- Serverless system ready for next integration stage

---

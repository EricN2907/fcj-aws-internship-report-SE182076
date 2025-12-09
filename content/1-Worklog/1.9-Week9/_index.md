---
title: "Week 9 Worklog"
date: 2025-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

- Design detailed project architecture
- Setup DynamoDB and data modeling
- Implement Authentication using Cognito
- Start developing Backend APIs

### Tasks to Execute This Week:

| **Date**          | **Task**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | **Start**  | **Finish** | **References**                   |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | -------------------------------- |
| Monday (03/11)    | - **Project Topic Selection:**<br>&emsp;+ Review project requirements<br>&emsp;+ Brainstorm project ideas<br>&emsp;+ Final decision: **Student Management System**<br>- List main features:<br>&emsp;+ User authentication (Cognito)<br>&emsp;+ CRUD operations<br>&emsp;+ Real-time notifications<br>- **Architecture Design:**<br>&emsp;+ Draw architecture diagram<br>&emsp;+ Define data flow<br>&emsp;+ List AWS services:<br>&emsp;&emsp;_ API Gateway → Lambda → DynamoDB<br>&emsp;&emsp;_ Cognito (Auth)<br>&emsp;&emsp;_ S3 (Storage)<br>&emsp;&emsp;_ CloudWatch (Monitoring)<br>- Document architecture decisions | 03/11/2025 | 03/11/2025 |                                  |
| Tuesday (04/11)   | - **DynamoDB Setup:**<br>&emsp;+ Create tables: Users, Classes, Subjects, Notifications<br>&emsp;+ Design partition keys and sort keys<br>&emsp;+ Setup GSI (Global Secondary Index)<br>&emsp;+ Test data access patterns<br>- Document data model                                                                                                                                                                                                                                                                                                                                                                           | 04/11/2025 | 04/11/2025 | DynamoDB Best Practices          |
| Wednesday (05/11) | - **Cognito Setup:**<br>&emsp;+ Create User Pool<br>&emsp;+ Configure sign-in options<br>&emsp;+ Setup password policies<br>&emsp;+ Create App Client<br>&emsp;+ Test authentication flow<br>- Document Cognito configuration                                                                                                                                                                                                                                                                                                                                                                                                | 05/11/2025 | 05/11/2025 | Cognito User Pools Documentation |
| Thursday (06/11)  | - **Backend Project Setup:**<br>&emsp;+ Initialize Java Spring Boot project<br>&emsp;+ Add AWS SDK dependencies<br>&emsp;+ Configure Maven for Lambda deployment<br>&emsp;+ Setup project structure<br>&emsp;+ Create Lambda Handler                                                                                                                                                                                                                                                                                                                                                                                         | 06/11/2025 | 06/11/2025 | Spring Boot Lambda Docs          |
| Friday (07/11)    | - **Implement Authentication APIs:**<br>&emsp;+ POST /auth/signup<br>&emsp;+ POST /auth/login<br>&emsp;+ POST /auth/refresh-token<br>&emsp;+ GET /auth/user-info<br>- Test Cognito integration                                                                                                                                                                                                                                                                                                                                                                                                                               | 07/11/2025 | 07/11/2025 | Cognito Authentication Guide     |

### Week 9 Achievements:

- Completed detailed architecture and data flow diagrams
- Set up DynamoDB (tables, partition/sort keys, GSI) and validated CRUD operations
- Configured Cognito User Pool and stable authentication flow
- Initialized backend project (Spring Boot) with Lambda handlers
- Authentication and user management endpoints are ready for further development

---

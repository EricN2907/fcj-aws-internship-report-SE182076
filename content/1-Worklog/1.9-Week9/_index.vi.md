---
title: "Worklog Tuần 9"
date: 2025-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

- Thiết kế Architecture chi tiết cho project
- Setup DynamoDB và data modeling
- Implement Authentication với Cognito
- Bắt đầu develop Backend API

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                                           |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | ---------------------------------------------------------------------------------------------------------------- |
| Thứ 2 (03/11) | - **Project Topic Selection:**<br>&emsp;+ Review project requirements<br>&emsp;+ Brainstorm project ideas<br>&emsp;+ Quyết định topic: **Student Management System**<br>- List các features chính:<br>&emsp;+ User authentication (Cognito)<br>&emsp;+ CRUD operations<br>&emsp;+ Real-time notifications<br>- **Architecture Design:**<br>&emsp;+ Vẽ architecture diagram<br>&emsp;+ Define data flow<br>&emsp;+ List AWS services:<br>&emsp;&emsp;_ API Gateway → Lambda → DynamoDB<br>&emsp;&emsp;_ Cognito (Auth)<br>&emsp;&emsp;_ S3 (Storage)<br>&emsp;&emsp;_ CloudWatch (Monitoring)<br>- Document architecture decisions | 03/11/2025  | 03/11/2025     |                                                                                                                  |
| Thứ 3 (04/11) | - **DynamoDB Setup:**<br>&emsp;+ Tạo tables: Users, Classes, Subjects, Notifications<br>&emsp;+ Design partition keys và sort keys<br>&emsp;+ Setup GSI (Global Secondary Index)<br>&emsp;+ Test data access patterns<br>- Document data model                                                                                                                                                                                                                                                                                                                                                                                    | 04/11/2025  | 04/11/2025     | [DynamoDB Best Practices](https://docs.aws.amazon.com/dynamodb/latest/developerguide/best-practices.html)        |
| Thứ 4 (05/11) | - **Cognito Setup:**<br>&emsp;+ Tạo User Pool<br>&emsp;+ Configure sign-in options<br>&emsp;+ Setup password policies<br>&emsp;+ Tạo App Client<br>&emsp;+ Test authentication flow<br>- Document Cognito configuration                                                                                                                                                                                                                                                                                                                                                                                                           | 05/11/2025  | 05/11/2025     | [Cognito User Pools](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html) |
| Thứ 5 (06/11) | - **Backend Project Setup:**<br>&emsp;+ Initialize Java Spring Boot project<br>&emsp;+ Add AWS SDK dependencies<br>&emsp;+ Configure Maven for Lambda deployment<br>&emsp;+ Setup project structure<br>&emsp;+ Create Lambda Handler                                                                                                                                                                                                                                                                                                                                                                                              | 06/11/2025  | 06/11/2025     | [Spring Boot Lambda](https://docs.aws.amazon.com/lambda/latest/dg/java-handler.html)                             |
| Thứ 6 (07/11) | - **Implement Authentication APIs:**<br>&emsp;+ POST /auth/signup<br>&emsp;+ POST /auth/login<br>&emsp;+ POST /auth/refresh-token<br>&emsp;+ GET /auth/user-info<br>- Test với Cognito integration                                                                                                                                                                                                                                                                                                                                                                                                                                | 07/11/2025  | 07/11/2025     | [Cognito Authentication](https://docs.aws.amazon.com/cognito/latest/developerguide/authentication-flow.html)     |

### Kết quả đạt được tuần 9:

- Hoàn thiện kiến trúc chi tiết và sơ đồ data flow cho project.
- Thiết lập DynamoDB (tables, partition/sort keys, GSI) và kiểm thử CRUD.
- Cấu hình Cognito User Pool và xác thực hoạt động ổn định.
- Khởi tạo project backend (Spring Boot) và handler Lambda.
- Các endpoint authentication và user management sẵn sàng để tiếp tục phát triển.

---

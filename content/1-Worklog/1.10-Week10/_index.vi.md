---
title: "Worklog Tuần 10"
date: 2025-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

- Hoàn thiện Backend APIs cho các features chính
- Deploy Lambda và API Gateway
- Tham gia AWS Cloud Mastery Series #1
- Setup CloudWatch monitoring

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                                                                                                                                                | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo** |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | ---------------------- |
| Thứ 2 (10/11) | - **Implement User Management APIs:**<br>&emsp;+ GET /users<br>&emsp;+ GET /users/{id}<br>&emsp;+ POST /users<br>&emsp;+ PUT /users/{id}<br>&emsp;+ DELETE /users/{id}<br>- Test CRUD operations<br>- Viết báo cáo tuần 9<br>- **Implement Class Management APIs:**<br>&emsp;+ GET /classes<br>&emsp;+ GET /classes/{id}<br>&emsp;+ POST /classes<br>&emsp;+ PUT /classes/{id}<br>&emsp;+ DELETE /classes/{id}<br>&emsp;+ GET /classes/{id}/students<br>- Test với DynamoDB | 10/11/2025  | 10/11/2025     | -                      |
| Thứ 3 (11/11) | - **Implement Subject Management APIs:**<br>&emsp;+ GET /subjects<br>&emsp;+ GET /subjects/{id}<br>&emsp;+ POST /subjects<br>&emsp;+ PUT /subjects/{id}<br>&emsp;+ DELETE /subjects/{id}<br>- Implement business logic và validation                                                                                                                                                                                                                                        | 11/11/2025  | 11/11/2025     | -                      |
| Thứ 4 (12/11) | - **Build và Package Lambda:**<br>&emsp;+ Configure pom.xml với maven-shade-plugin<br>&emsp;+ Build JAR: `mvn clean package`<br>&emsp;+ Test locally nếu có thể<br>&emsp;+ Verify JAR size (< 50MB recommended)                                                                                                                                                                                                                                                             | 12/11/2025  | 12/11/2025     | -                      |
| Thứ 5 (13/11) | - **Deploy Lambda Function:**<br>&emsp;+ Tạo Lambda function trên AWS Console<br>&emsp;+ Upload JAR file<br>&emsp;+ Configure Handler, Memory (1024MB), Timeout (30s)<br>&emsp;+ Setup IAM Role với DynamoDB permissions<br>&emsp;+ Test Lambda với sample events                                                                                                                                                                                                           | 13/11/2025  | 13/11/2025     | -                      |
| Thứ 6 (14/11) | - **Create API Gateway:**<br>&emsp;+ Tạo HTTP API hoặc REST API<br>&emsp;+ Configure route: `ANY /{proxy+}`<br>&emsp;+ Enable CORS<br>&emsp;+ Deploy stage: prod<br>&emsp;+ Test các endpoints<br>- Document API Gateway URL                                                                                                                                                                                                                                                | 14/11/2025  | 14/11/2025     | -                      |

### Kết quả đạt được tuần 10:

- APIs backend (Class, Subject) hoàn thiện và hoạt động ổn định.
- Lambda + API Gateway đã triển khai và sẵn sàng tích hợp frontend.
- Kiểm thử và logging (CloudWatch) đã thiết lập.
- Tham dự workshop AWS, nghiên cứu AI/ML cho tính năng tương lai.
- Hệ thống serverless sẵn sàng cho giai đoạn tích hợp tiếp theo.

---

---
title: "Worklog Tuần 5"
date: 2025-10-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

- Nắm vững Serverless Architectures (Lambda, API Gateway)
- Tìm hiểu Container Services (ECS, Fargate)
- Học về Monitoring và Logging (CloudWatch)

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                                              | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                                         |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | -------------------------------------------------------------------------------------------------------------- |
| Thứ 2 (06/10) | - So sánh các database services:<br>&emsp;+ RDS vs DynamoDB vs Aurora<br>&emsp;+ Use cases cho từng loại<br>- Ôn tập và viết báo cáo tuần 4<br>- Tìm hiểu AWS Lambda:<br>&emsp;+ Serverless concepts<br>&emsp;+ Lambda function basics<br>&emsp;+ Triggers & Event Sources<br>&emsp;+ Execution Role & Permissions<br>- **Thực hành:** Tạo Lambda function với S3 trigger | 06/10/2025  | 06/10/2025     | [Lambda Developer Guide](https://docs.aws.amazon.com/lambda/)                                                  |
| Thứ 3 (07/10) | - Tìm hiểu API Gateway:<br>&emsp;+ REST API vs HTTP API<br>&emsp;+ Integration types<br>&emsp;+ CORS configuration<br>&emsp;+ API Keys & Usage Plans<br>- **Thực hành:** Tạo REST API với Lambda integration                                                                                                                                                              | 07/10/2025  | 07/10/2025     | [API Gateway Guide](https://docs.aws.amazon.com/apigateway/)                                                   |
| Thứ 4 (08/10) | - Lambda nâng cao:<br>&emsp;+ Environment Variables<br>&emsp;+ Layers<br>&emsp;+ VPC Configuration<br>&emsp;+ Cold Start Optimization<br>- **Thực hành:** Lambda kết nối RDS trong VPC                                                                                                                                                                                    | 08/10/2025  | 08/10/2025     | [Lambda Best Practices](https://docs.aws.amazon.com/lambda/latest/dg/best-practices.html)                      |
| Thứ 5 (09/10) | - Tìm hiểu Container Services:<br>&emsp;+ Docker basics review<br>&emsp;+ ECS (Elastic Container Service)<br>&emsp;+ Fargate vs EC2 Launch Type<br>&emsp;+ Task Definitions<br>- **Thực hành:** Deploy container trên Fargate                                                                                                                                             | 09/10/2025  | 09/10/2025     | [ECS Documentation](https://docs.aws.amazon.com/ecs/)<br>[Fargate Guide](https://docs.aws.amazon.com/fargate/) |
| Thứ 6 (10/10) | - Tìm hiểu CloudWatch:<br>&emsp;+ Metrics & Dimensions<br>&emsp;+ Logs & Log Groups<br>&emsp;+ Alarms & Notifications (SNS)<br>&emsp;+ CloudWatch Insights<br>- **Thực hành:** Setup monitoring cho Lambda và EC2                                                                                                                                                         | 10/10/2025  | 10/10/2025     | [CloudWatch User Guide](https://docs.aws.amazon.com/cloudwatch/)                                               |

### Kết quả đạt được tuần 5:

- Xây dựng serverless API (API Gateway + Lambda + DynamoDB) hoạt động ổn định.
- Triển khai monitoring và logging với CloudWatch.
- Đã thử nghiệm container deployment trên Fargate cơ bản.
- Tối ưu hiệu năng Lambda và xử lý lỗi.
- Hệ thống sẵn sàng cho giai đoạn tích hợp frontend.

---

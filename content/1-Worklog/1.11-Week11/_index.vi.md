---
title: "Worklog Tuần 11"
date: 2025-11-16
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

- Setup CloudWatch monitoring và alarms
- Implement Notification system
- Tham gia AWS Cloud Mastery Series #2 (DevOps)
- Optimize Lambda performance

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                           | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                 |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------- | -------------- | -------------------------------------------------------------------------------------- |
| Thứ 2 (17/11) | **AWS Cloud Mastery Series #2 – DevOps on AWS**<br>_Time: 08:30 – 17:00_<br>- Tham dự full-day workshop<br>- Learn CodePipeline, CodeBuild, CodeDeploy<br>- Hands-on labs về CI/CD<br>- Plan CI/CD cho project                                         | 17/11/2025  | 17/11/2025     | -                                                                                      |
| Thứ 3 (18/11) | - **Setup CloudWatch Monitoring:**<br>&emsp;+ Verify Lambda log groups<br>&emsp;+ Create custom metrics<br>&emsp;+ Setup CloudWatch Insights queries<br>&emsp;+ Create monitoring dashboard                                                            | 18/11/2025  | 18/11/2025     | [CloudWatch Guide](https://docs.aws.amazon.com/cloudwatch/)                            |
| Thứ 4 (19/11) | - **Configure CloudWatch Alarms:**<br>&emsp;+ Lambda error alarm (threshold > 5)<br>&emsp;+ Lambda duration alarm<br>&emsp;+ API Gateway 5xx alarm<br>&emsp;+ DynamoDB throttle alarm<br>- Setup SNS notifications                                     | 19/11/2025  | 19/11/2025     |                                                                                        |
| Thứ 5 (20/11) | - **Implement Notifications APIs:**<br>&emsp;+ POST /notifications (create)<br>&emsp;+ GET /notifications (list)<br>&emsp;+ GET /notifications/{id}<br>&emsp;+ PUT /notifications/{id}/read (mark as read)<br>- Integrate với DynamoDB table           | 20/11/2025  | 20/11/2025     | -                                                                                      |
| Thứ 6 (21/11) | - **Lambda Performance Optimization:**<br>&emsp;+ Analyze cold start metrics<br>&emsp;+ Optimize dependencies<br>&emsp;+ Implement connection pooling cho DynamoDB<br>&emsp;+ Consider Provisioned Concurrency<br>- Benchmark performance improvements | 21/11/2025  | 21/11/2025     | [Lambda Performance](https://docs.aws.amazon.com/lambda/latest/dg/best-practices.html) |

### Kết quả đạt được tuần 11:

- Tham dự workshop AWS, nắm vững CI/CD và DevOps.
- Thiết lập CloudWatch monitoring, dashboard và cảnh báo tự động.
- Hoàn thiện APIs thông báo, tối ưu DynamoDB, hỗ trợ phân trang.
- Tối ưu hiệu năng Lambda, giảm cold start, cải thiện thời gian xử lý.
- Hệ thống sẵn sàng kiểm thử tải thực tế, đảm bảo giám sát và cảnh báo.

---

---
title: "Worklog Tuần 12"
date: 2025-11-23
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

- Setup Security services (WAF, GuardDuty)
- Implement CI/CD Pipeline
- Tham gia AWS Cloud Mastery Series #3 (Security)
- Setup CloudFront và Route53

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                               | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                                          |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | --------------------------------------------------------------------------------------------------------------- |
| Thứ 2 (24/11) | - **Setup WAF (Web Application Firewall):**<br>&emsp;+ Tạo WAF Web ACL<br>&emsp;+ Add AWS Managed Rules:<br>&emsp;&emsp;_ Core Rule Set<br>&emsp;&emsp;_ Known Bad Inputs<br>&emsp;&emsp;\* SQL Injection Protection<br>&emsp;+ Configure rate limiting (2000 req/5min)<br>- Associate WAF với API Gateway | 24/11/2025  | 24/11/2025     | [WAF Guide](https://docs.aws.amazon.com/waf/)                                                                   |
| Thứ 3 (25/11) | - **Enable GuardDuty:**<br>&emsp;+ Activate GuardDuty<br>&emsp;+ Review findings<br>&emsp;+ Setup GuardDuty notifications<br>- **Enable Security Hub:**<br>&emsp;+ Centralized security view<br>&emsp;+ Enable security standards                                                                          | 25/11/2025  | 25/11/2025     | [GuardDuty](https://docs.aws.amazon.com/guardduty/)<br>[Security Hub](https://docs.aws.amazon.com/securityhub/) |
| Thứ 4 (26/11) | - **Setup S3 Bucket cho Artifacts:**<br>&emsp;+ Tạo bucket với versioning<br>&emsp;+ Configure lifecycle policies<br>- **Create CodeBuild Project:**<br>&emsp;+ Source: GitLab/GitHub<br>&emsp;+ Environment: Java 17<br>&emsp;+ Buildspec file cho backend<br>&emsp;+ Test build process                  | 26/11/2025  | 26/11/2025     | [CodeBuild Guide](https://docs.aws.amazon.com/codebuild/)                                                       |
| Thứ 5 (27/11) | - **Create CodePipeline:**<br>&emsp;+ Source stage: GitLab webhook<br>&emsp;+ Build stage: CodeBuild project<br>&emsp;+ Deploy stage: Lambda function update<br>- Test automated deployment flow<br>- Document CI/CD process                                                                               | 27/11/2025  | 27/11/2025     | [CodePipeline](https://docs.aws.amazon.com/codepipeline/)                                                       |
| Thứ 6 (28/11) | - **Setup CloudFront Distribution:**<br>&emsp;+ Origin: API Gateway<br>&emsp;+ Configure caching behaviors<br>&emsp;+ HTTPS only<br>&emsp;+ Associate WAF Web ACL<br>- Test CDN performance<br>- Measure latency improvements                                                                              | 28/11/2025  | 28/11/2025     | [CloudFront Guide](https://docs.aws.amazon.com/cloudfront/)                                                     |

### Kết quả đạt được tuần 12:

- Đã triển khai WAF, GuardDuty, Security Hub, đảm bảo bảo mật và tuân thủ.
- Thiết lập CI/CD tự động, build nhanh, deploy không downtime.
- CloudFront phân phối toàn cầu, cải thiện hiệu năng API.
- Tham gia workshop AWS, áp dụng kiến thức bảo mật mới.
- Kiến trúc đạt chuẩn production, checklist bảo mật hoàn thành.

---

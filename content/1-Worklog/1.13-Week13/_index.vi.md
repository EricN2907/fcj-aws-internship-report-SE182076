---
title: "Worklog Tuần 13"
date: 2025-11-30
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

### Mục tiêu tuần 13:

- Hoàn thiện project và testing toàn diện
- Setup Route53 và custom domain (nếu có)
- Cost optimization review
- Chuẩn bị presentation và documentation

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                                          | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                           |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | ---------------------------------------------------------------- |
| Thứ 2 (01/12) | - **Route53 Setup (Optional):**<br>&emsp;+ Tạo Hosted Zone<br>&emsp;+ Configure A record cho CloudFront<br>&emsp;+ Request SSL certificate (ACM)<br>&emsp;+ DNS validation<br>- **Comprehensive Testing:**<br>&emsp;+ API endpoint testing<br>&emsp;+ Authentication flow testing<br>&emsp;+ Error handling validation                                                | 01/12/2025  | 01/12/2025     | [Route53 Guide](https://docs.aws.amazon.com/route53/)            |
| Thứ 3 (02/12) | - **Integration Testing:**<br>&emsp;+ End-to-end user workflows<br>&emsp;+ Edge cases testing<br>&emsp;+ Load testing với sample data<br>&emsp;+ Security testing (OWASP Top 10)<br>- Document test results và findings                                                                                                                                               | 02/12/2025  | 02/12/2025     | -                                                                |
| Thứ 4 (03/12) | - **Cost Optimization Review:**<br>&emsp;+ Analyze AWS Cost Explorer<br>&emsp;+ Review current spending<br>&emsp;+ Identify optimization opportunities:<br>&emsp;&emsp;_ Lambda memory sizing<br>&emsp;&emsp;_ DynamoDB capacity mode<br>&emsp;&emsp;_ S3 lifecycle policies<br>&emsp;&emsp;_ CloudWatch log retention<br>- Document cost optimizations implemented   | 03/12/2025  | 03/12/2025     | [Cost Optimization](https://aws.amazon.com/aws-cost-management/) |
| Thứ 5 (04/12) | - **Project Documentation:**<br>&emsp;+ Architecture diagram finalization<br>&emsp;+ API documentation (Swagger/OpenAPI)<br>&emsp;+ README.md comprehensive<br>&emsp;+ Troubleshooting guide<br>- Code cleanup và commenting                                                                                                                                          | 04/12/2025  | 04/12/2025     |                                                                  |
| Thứ 6 (05/12) | - **Presentation Preparation:**<br>&emsp;+ Create presentation slides:<br>&emsp;&emsp;_ Project overview<br>&emsp;&emsp;_ Architecture design<br>&emsp;&emsp;_ AWS services used<br>&emsp;&emsp;_ Security implementations<br>&emsp;&emsp;_ Performance metrics<br>&emsp;&emsp;_ Challenges & solutions<br>&emsp;&emsp;\* Demo preparation<br>- Practice presentation | 05/12/2025  | 05/12/2025     |                                                                  |

### Kết quả đạt được tuần 13:

- Đã triển khai production, SSL và DNS hoạt động ổn định, dịch vụ chạy tốt.
- Hoàn thành kiểm thử toàn diện: unit, integration, end-to-end, bảo mật, hiệu năng.
- Tối ưu chi phí AWS, thiết lập cảnh báo ngân sách và tag chi phí.
- Bộ tài liệu hoàn chỉnh: kiến trúc, API, hướng dẫn triển khai, troubleshooting, README.
- Slide trình bày chuyên nghiệp, demo trực tiếp các tính năng chính.

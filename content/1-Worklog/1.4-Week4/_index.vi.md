---
title: "Worklog Tuần 4"
date: 2025-09-28
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

- Nắm vững kiến thức về Storage Services (S3, EFS, EBS)
- Tìm hiểu Database Services (RDS, DynamoDB)
- Học về High-Performing Architectures

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                                                                                                                 | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                                                 |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Thứ 2 (29/09) | - **Lab tổng hợp:** Thiết kế và deploy kiến trúc High Availability:<br>&emsp;+ Multi-AZ VPC<br>&emsp;+ ALB + Auto Scaling<br>&emsp;+ Route 53 health check<br>- Viết báo cáo tuần 3<br>- Tìm hiểu S3 심화:<br>&emsp;+ Storage Classes (Standard, IA, Glacier, Deep Archive)<br>&emsp;+ Lifecycle Policies<br>&emsp;+ Versioning & Object Lock<br>&emsp;+ S3 Performance Optimization<br>- **Thực hành:** Cấu hình S3 lifecycle và versioning | 29/09/2025  | 29/09/2025     | [S3 User Guide](https://docs.aws.amazon.com/s3/)<br>[S3 Storage Classes](https://aws.amazon.com/s3/storage-classes/)   |
| Thứ 3 (30/09) | - Tìm hiểu EFS và FSx:<br>&emsp;+ EFS vs EBS vs S3<br>&emsp;+ EFS Performance Modes<br>&emsp;+ Mount targets<br>- **Thực hành:** Mount EFS vào EC2 instances                                                                                                                                                                                                                                                                                 | 30/09/2025  | 30/09/2025     | [EFS Documentation](https://docs.aws.amazon.com/efs/)                                                                  |
| Thứ 4 (01/10) | - Tìm hiểu RDS:<br>&emsp;+ RDS Engines (MySQL, PostgreSQL, Aurora)<br>&emsp;+ Multi-AZ Deployments<br>&emsp;+ Read Replicas<br>&emsp;+ Backup & Snapshots<br>- **Thực hành:** Tạo RDS MySQL Multi-AZ                                                                                                                                                                                                                                         | 01/10/2025  | 01/10/2025     | [RDS User Guide](https://docs.aws.amazon.com/rds/)                                                                     |
| Thứ 5 (02/10) | - Tìm hiểu DynamoDB:<br>&emsp;+ NoSQL concepts<br>&emsp;+ Partition Keys & Sort Keys<br>&emsp;+ GSI & LSI<br>&emsp;+ On-Demand vs Provisioned Capacity<br>- **Thực hành:** Tạo DynamoDB table với GSI                                                                                                                                                                                                                                        | 02/10/2025  | 02/10/2025     | [DynamoDB Developer Guide](https://docs.aws.amazon.com/dynamodb/)                                                      |
| Thứ 6 (03/10) | - Tìm hiểu **High-Performing Architectures** (Phần 1):<br>&emsp;+ Caching Strategies (CloudFront, ElastiCache)<br>&emsp;+ Content Delivery<br>&emsp;+ Read Replicas<br>- **Thực hành:** Setup CloudFront với S3 origin                                                                                                                                                                                                                       | 03/10/2025  | 03/10/2025     | [CloudFront Guide](https://docs.aws.amazon.com/cloudfront/)<br>[ElastiCache](https://docs.aws.amazon.com/elasticache/) |

### Kết quả đạt được tuần 4:

- Hiểu và cấu hình S3 lifecycle, versioning và storage classes để tối ưu chi phí.
- Thực hành RDS Multi-AZ và nắm các chiến lược sao lưu/restore.
- Thiết kế DynamoDB (partition/sort key, GSI) cho access patterns.
- Triển khai CloudFront để tối ưu phân phối nội dung.
- Sẵn sàng cho thiết kế kiến trúc hiệu năng cao.

---

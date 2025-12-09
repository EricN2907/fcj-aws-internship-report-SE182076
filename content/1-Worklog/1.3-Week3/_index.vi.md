---
title: "Worklog Tuần 3"
date: 2025-09-21
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

- Nắm vững kiến thức về Resilient Architectures
- Tìm hiểu Load Balancing và Auto Scaling
- Học về Route 53 và DNS

### Các công việc cần triển khai trong tuần này:

| **Ngày**      | **Nhiệm vụ**                                                                                                                                                                                                                                                                                                                                          | **Bắt đầu** | **Hoàn thành** | **Tài liệu tham khảo**                                                                                                       |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Thứ 2 (22/09) | - Tìm hiểu EC2 Storage:<br>&emsp;+ EBS Volume Types<br>&emsp;+ Snapshots<br>&emsp;+ Instance Store<br>- Ôn tập và viết báo cáo tuần 2<br>- Tìm hiểu **Resilient Architectures** (Phần 1):<br>&emsp;+ Multi-AZ Architecture<br>&emsp;+ Fault Tolerance vs High Availability<br>&emsp;+ RTO & RPO concepts<br>- **Thực hành:** Deploy EC2 trên Multi-AZ | 22/09/2025  | 22/09/2025     | [AWS Resilience Hub](https://docs.aws.amazon.com/resilience-hub/)<br>[Multi-AZ Design](https://aws.amazon.com/architecture/) |
| Thứ 3 (23/09) | - Tìm hiểu Elastic Load Balancer:<br>&emsp;+ ALB (Application Load Balancer)<br>&emsp;+ NLB (Network Load Balancer)<br>&emsp;+ Target Groups<br>&emsp;+ Health Checks<br>- **Thực hành:** Tạo ALB cho 2 EC2 instances                                                                                                                                 | 23/09/2025  | 23/09/2025     | [ELB Documentation](https://docs.aws.amazon.com/elasticloadbalancing/)                                                       |
| Thứ 4 (24/09) | - Tìm hiểu Auto Scaling:<br>&emsp;+ Launch Templates<br>&emsp;+ Auto Scaling Groups<br>&emsp;+ Scaling Policies (Target Tracking, Step Scaling)<br>&emsp;+ Scaling Cooldown<br>- **Thực hành:** Tạo Auto Scaling Group với scaling policy                                                                                                             | 24/09/2025  | 24/09/2025     | [Auto Scaling Guide](https://docs.aws.amazon.com/autoscaling/ec2/userguide/)                                                 |
| Thứ 5 (25/09) | - Tìm hiểu Route 53:<br>&emsp;+ DNS fundamentals<br>&emsp;+ Routing Policies (Simple, Weighted, Failover, Geolocation)<br>&emsp;+ Health Checks<br>- **Thực hành:** Cấu hình Route 53 với Failover routing                                                                                                                                            | 25/09/2025  | 25/09/2025     | [Route 53 Documentation](https://docs.aws.amazon.com/route53/)                                                               |
| Thứ 6 (26/09) | - Tìm hiểu Disaster Recovery Strategies:<br>&emsp;+ Backup & Restore<br>&emsp;+ Pilot Light<br>&emsp;+ Warm Standby<br>&emsp;+ Multi-Site Active/Active<br>- So sánh RTO/RPO cho từng strategy                                                                                                                                                        | 26/09/2025  | 26/09/2025     | [DR Strategies](https://docs.aws.amazon.com/whitepapers/latest/disaster-recovery-workloads-on-aws/)                          |

### Kết quả đạt được tuần 3:

- Thiết kế và triển khai kiến trúc High-Availability (Multi-AZ, ALB, Auto Scaling).
- Cấu hình Route 53 với health checks và cơ chế failover.
- Thiết lập và kiểm thử load balancing và health checks.
- Áp dụng Auto Scaling với chính sách dựa trên metrics.
- Sẵn sàng cho các kịch bản Disaster Recovery.

---

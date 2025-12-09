---
title: "Event 5"
date: 2025-11-29
weight: 5
chapter: false
pre: "<b> 4.5. </b>"
---

# Báo cáo chuyên đề: Bảo mật Đám mây theo chuẩn AWS Well-Architected

## 1. Mục tiêu tham dự
Trong bối cảnh các mối đe dọa an ninh mạng ngày càng tinh vi, buổi workshop này là cơ hội then chốt để tôi củng cố kiến thức về **Trụ cột Bảo mật (Security Pillar)**. Mục tiêu của tôi bao gồm:
- Thấm nhuần các tư duy bảo mật hiện đại: **Zero Trust**, **Least Privilege** (Đặc quyền tối thiểu) và **Defense in Depth** (Phòng thủ chiều sâu).
- Làm chủ 5 lĩnh vực bảo mật trọng yếu: Quản lý danh tính (IAM), Phát hiện mối đe dọa, Bảo vệ hạ tầng, Bảo vệ dữ liệu và Ứng phó sự cố.
- Học hỏi kinh nghiệm thực chiến từ các chuyên gia để nhận diện và phòng chống các kịch bản tấn công phổ biến tại thị trường Việt Nam.

## 2. Thông tin sự kiện
- **Thời gian:** 08:30 – 12:00 | Thứ Bảy, 29/11/2025.
- **Địa điểm:** Tầng 26, Bitexco Financial Tower, Quận 1, TP. HCM.
- **Diễn giả:** Đội ngũ AWS Cloud Club Captains, AWS Community Builders và khách mời đặc biệt **Mendel Grabski** (Cloud Security Architect).

## 3. Kiến thức cốt lõi

### Quản lý Danh tính & Truy cập (IAM)
- **Identity is the new Firewall:** Trong môi trường Cloud-native, việc quản lý danh tính quan trọng hơn cả tường lửa mạng truyền thống.
- **Zero Trust:** Loại bỏ tư duy "tin cậy mạng nội bộ". Mọi yêu cầu truy cập đều phải được xác thực nghiêm ngặt.
- **Hiện đại hóa xác thực:** Kiên quyết loại bỏ Access Keys dài hạn, thay thế bằng **IAM Roles** và **Identity Center (SSO)**. Sử dụng công cụ **Access Analyzer** để rà soát và loại bỏ các quyền dư thừa.

### Phát hiện & Bảo vệ Hạ tầng
- **Tầm nhìn tập trung:** Sử dụng **AWS Security Hub** làm trung tâm chỉ huy, tổng hợp cảnh báo từ GuardDuty, Inspector và Macie.
- **Defense in Depth:** Thiết lập nhiều lớp bảo vệ từ Network (VPC, Security Groups) đến Edge (WAF, Shield).
- **Encryption Everywhere:** Mã hóa là bắt buộc. Sử dụng KMS cho dữ liệu lưu trữ (At-rest) và TLS 1.2+ cho dữ liệu truyền tải (In-transit).

### Tự động hóa Ứng phó sự cố (Automated IR)
- **Quy trình IR:** Chuẩn hóa theo vòng đời: Chuẩn bị → Phát hiện → Khoanh vùng → Khôi phục.
- **Automation:** Thay vì xử lý thủ công chậm chạp, sử dụng **Lambda** và **Step Functions** để tự động phản ứng (ví dụ: tự động thu hồi quyền IAM ngay khi phát hiện hành vi bất thường).

## 4. Tư duy & Bài học
- **Security by Design:** Bảo mật không phải là tính năng bổ sung (add-on), mà phải được tích hợp ngay từ dòng code đầu tiên.
- **Assume Breach:** Luôn thiết kế hệ thống với giả định rằng "chúng ta đã bị tấn công". Từ đó, tập trung vào việc giảm thiểu phạm vi ảnh hưởng (Blast Radius) và tối ưu tốc độ khôi phục.
- **Hạ tầng bất biến (Immutable Infrastructure):** Hạn chế tối đa việc SSH vào server sửa lỗi; thay vào đó hãy thay thế bằng server mới "sạch" đã được vá lỗi.

## 5. Kế hoạch hành động (Action Plan)
Áp dụng ngay các kiến thức đã học để gia cố bảo mật cho dự án **Serverless Student Management**:
1.  **Refactor IAM:** Rà soát toàn bộ policy, loại bỏ quyền `*:*` và hardcoded credentials. Chuyển sang dùng IAM Roles cho các Lambda functions.
2.  **Quản lý Secrets:** Di dời toàn bộ Database Password và API Keys từ file cấu hình `.env` cục bộ sang **AWS Systems Manager Parameter Store** để quản lý tập trung và an toàn.
3.  **Giám sát an ninh:** Kích hoạt **Amazon GuardDuty** (tận dụng Free Tier) để phát hiện sớm các hành vi đáng ngờ (như đào coin trái phép trên tài khoản thực tập).
4.  **Bảo vệ dữ liệu:** Bật mặc định mã hóa Server-Side Encryption (SSE-S3) cho tất cả S3 Buckets chứa hồ sơ sinh viên.

## 6. Trải nghiệm tham dự
Sự kiện mang lại góc nhìn thực tế và cấp bách về bảo mật đám mây. Các phần demo về **Validate IAM Policy** hay **Automated Incident Response** đã minh chứng rõ ràng sức mạnh của tự động hóa trong bảo mật. Đặc biệt, các thảo luận về Use-case thực tế tại Việt Nam giúp tôi ý thức sâu sắc hơn về trách nhiệm bảo vệ thông tin xác thực người dùng.

![All members participated](/images/4-EventParticipated/4.5-Event5/Image_5.2)
![Identity & Access Management](/images/4-EventParticipated/4.5-Event5/Image_5.1)
![The Badging Journey](/images/4-EventParticipated/4.5-Event5/Image_5.3)
![Multi Layer Security against Attack Vectors](/images/4-EventParticipated/4.5-Event5/Image_5.4)
![Special Guest](/images/4-EventParticipated/4.5-Event5/Image_5.5)

> **Tổng kết:** Sự kiện đã chuyển đổi tư duy của tôi từ "xây dựng cho chạy được" sang "xây dựng an toàn và bền vững". Đây là bước chuẩn bị quan trọng trước khi tôi đưa bất kỳ ứng dụng nào ra môi trường Production.
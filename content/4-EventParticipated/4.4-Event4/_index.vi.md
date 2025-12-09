---
title: "Event 4"
date: 2025-09-09
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---


# Báo cáo tổng kết: AWS Cloud Mastery Series #2 – DevOps on AWS

## 1. Mục tiêu tham dự
Tham gia sự kiện này, tôi đặt ra các mục tiêu trọng tâm để nâng cao năng lực kỹ thuật:
- Nắm vững tư duy cốt lõi của DevOps và cách đo lường hiệu quả qua bộ chỉ số DORA.
- Làm chủ quy trình xây dựng CI/CD pipeline toàn diện (end-to-end) trên hệ sinh thái AWS.
- Phân tích và lựa chọn công cụ Infrastructure as Code (IaC) tối ưu: CloudFormation hay AWS CDK?
- Tìm hiểu chiến lược Container hóa với Amazon ECS, EKS và App Runner.
- Triển khai giải pháp Observability (Khả năng quan sát) chuyên sâu với CloudWatch và AWS X-Ray.

## 2. Thông tin sự kiện
- **Thời gian:** 08:30 – 17:00, Thứ Hai, ngày 17/11/2025.
- **Địa điểm:** Tầng 26, Tòa nhà tài chính Bitexco, Quận 1, TP. HCM.
- **Diễn giả:** Các chuyên gia từ AWS Community Builders (Trương Quang Tinh, Kha Van, Bảo Huỳnh, Thịnh Nguyễn, Vi Trần).

## 3. Nội dung chuyên môn

### Tư duy DevOps & Đo lường hiệu suất
- **Văn hóa hợp nhất:** Xóa bỏ ranh giới giữa Dev và Ops, hướng tới mô hình trách nhiệm chia sẻ.
- **DORA Metrics:** 4 thước đo "vàng" cho sức khỏe dự án: Tần suất triển khai (DF), Thời gian thay đổi (LT), Thời gian khôi phục (MTTR) và Tỷ lệ lỗi (CFR).

### Hệ sinh thái CI/CD trên AWS
- **Source Control:** Quản lý mã nguồn với AWS CodeCommit, so sánh mô hình GitFlow và Trunk-based.
- **Orchestration:** Tự động hóa quy trình phát hành phần mềm bằng **AWS CodePipeline**.
- **Chiến lược Deploy:**
    - *Blue/Green:* Chạy song song hai môi trường để giảm rủi ro và downtime.
    - *Canary:* Phát hành thử nghiệm cho một nhóm nhỏ người dùng.
    - *Rolling:* Cập nhật cuốn chiếu từng phần hạ tầng.

### Infrastructure as Code (IaC)
- **AWS CloudFormation:** Tiếp cận theo hướng khai báo (Declarative) với JSON/YAML, mạnh về quản lý trạng thái (drift detection).
- **AWS CDK:** Tiếp cận theo hướng mệnh lệnh (Imperative), cho phép dùng ngôn ngữ lập trình (Java, TypeScript...) để định nghĩa hạ tầng, giúp tái sử dụng code hiệu quả hơn.

### Containers & Observability
- **Lựa chọn Compute:** Cân nhắc giữa sự kiểm soát chi tiết (Amazon ECS), chuẩn hóa Kubernetes (EKS) hoặc sự đơn giản, nhanh chóng (App Runner).
- **Giám sát toàn diện:** Kết hợp CloudWatch (Logs/Metrics) và AWS X-Ray để truy vết (tracing) lỗi trong kiến trúc Microservices phức tạp.

## 4. Bài học đúc kết

### Tư duy thiết kế hệ thống
- **Automate Everything:** Từ kiểm thử đến triển khai hạ tầng đều phải tự động hóa để loại bỏ lỗi con người.
- **Shift-Left Security:** Bảo mật phải được tích hợp ngay từ khâu viết code, không phải là bước cuối cùng.
- **Data-Driven:** Sử dụng DORA metrics làm kim chỉ nam để cải thiện quy trình.

### Kiến trúc & Hiện đại hóa
- **Immutable Infrastructure:** Không sửa chữa máy chủ đang chạy; thay thế hoàn toàn bằng máy chủ mới khi có thay đổi.
- **Pipeline Orchestration:** Thiết lập các cổng kiểm soát (approval gates) chặt chẽ trước khi lên Production.
- **Right-sizing:** Chọn công cụ đúng mục đích (ví dụ: dùng App Runner cho các web app đơn giản để tiết kiệm chi phí vận hành).

## 5. Kế hoạch hành động (Action Plan)

Sau workshop, tôi sẽ áp dụng kiến thức vào dự án thực tế:
1.  **Quy trình Git:** Chuyển sang mô hình **Trunk-based Development** để giảm xung đột code khi làm việc nhóm.
2.  **CI/CD Pipeline:** Thiết lập **AWS CodePipeline** cho dự án quản lý sinh viên, đảm bảo code được deploy tự động ngay khi merge.
3.  **Refactor hạ tầng:** Viết lại cấu hình DynamoDB và Lambda hiện tại bằng **AWS CDK** thay vì thao tác tay, giúp dễ dàng bảo trì và mở rộng.
4.  **Giám sát:** Cài đặt **CloudWatch Alarms** cảnh báo ngay lập tức khi API trả về lỗi 5xx.

## 6. Trải nghiệm & Cảm nhận

Sự kiện "DevOps on AWS" thực sự là mảnh ghép quan trọng giúp tôi kết nối tư duy Lập trình (Dev) và Vận hành (Ops). Không chỉ dừng lại ở lý thuyết, tôi đã được chứng kiến sức mạnh thực tế của việc tự động hóa:
- **Học từ chuyên gia:** Hiểu rõ những "cạm bẫy" thực tế khi triển khai DevOps và mô hình Trách nhiệm Chia sẻ.
- **Live Demo ấn tượng:** Tận mắt thấy AWS CDK triển khai cả một cụm VPC và ECS chỉ với lượng code rất ngắn gọn, cũng như khả năng "bắt bệnh" hệ thống tức thời của AWS X-Ray.
- **Networking:** Được định hướng rõ ràng hơn về lộ trình chinh phục chứng chỉ **AWS Certified DevOps Engineer – Professional**.

> **Kết luận:** "Infrastructure as Code" và "Observability" không còn là lựa chọn, mà là tiêu chuẩn bắt buộc. Sự kiện đã trang bị cho tôi tư duy cần thiết để xây dựng những hệ thống chuẩn Production: Tin cậy, Bảo mật và Dễ mở rộng.

![](/images/4-EventParticipated/4.4-Event4/Image_4.1.jpg)
![Warm-up with speaker Tinh Truong](/images/4-EventParticipated/4.4-Event4/Image_4.2.jpg)
![Infrastructure as Code (IaC)](/images/4-EventParticipated/4.4-Event4/Image_4.3.jpg)
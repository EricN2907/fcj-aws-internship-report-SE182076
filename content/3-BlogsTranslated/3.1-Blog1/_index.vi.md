---
title: "Blog 1"
date: 2025-09-09
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Đơn giản hóa canary bằng cách gộp (batch) nhiều URL trong Amazon CloudWatch Synthetics

**Tác giả:** Shree Chinnasamy  

**Ngày đăng:** 20 tháng 9 năm 2021  

**Danh mục:** [Amazon CloudWatch](https://aws.amazon.com/blogs/mt/category/management-tools/amazon-cloudwatch/), [Announcements](https://aws.amazon.com/blogs/mt/category/post-types/announcements/), [Foundational (100)](https://aws.amazon.com/blogs/mt/category/learning-levels/foundational-100/)

---

Bạn có thể sử dụng [Amazon CloudWatch Synthetics](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries.html) để tạo canary, các script có thể cấu hình và chạy theo lịch trình, nhằm giám sát các điểm cuối (endpoint) và hoạt động API của bạn. Canary đi theo các tuyến đường (routes) giống nhau và thực hiện các hành động giống như một khách hàng, điều này giúp bạn có thể xác minh liên tục trải nghiệm khách hàng ngay cả khi không có bất kỳ lưu lượng truy cập nào của khách hàng trên ứng dụng của mình. Bằng cách sử dụng canary, bạn có thể phát hiện sự cố trước khi khách hàng của bạn gặp phải.

Nếu canary của bạn sử dụng runtime version **syn-nodejs-puppeteer-3.1** hoặc mới hơn, bạn có thể sử dụng mẫu *Giám sát Nhịp tim (Heartbeat monitoring)* và xử lý theo lô (batch) nhiều URL trong một canary duy nhất, thay vì phải tạo nhiều canary riêng cho từng URL. Sau đó, bạn có thể xem trạng thái, thời lượng, ảnh chụp màn hình và lý do lỗi cho từng URL trong phần tóm tắt bước (step summary) của báo cáo chạy canary.

Vì CloudWatch Synthetics được tính phí dựa trên số lần chạy canary, nên việc gộp nhiều URL trong một canary cũng giúp giảm chi phí. (Hãy xem phần **Định giá** của bài đăng blog này để biết thêm chi tiết.)

## **Quy trình thực hiện**

Trong bài đăng blog này, tôi trình bày giá trị đề xuất (value proposition) của việc xử lý theo lô (batching) nhiều URL trong một canary duy nhất. Ví dụ trong bài, canary của tôi sẽ giám sát nhiều URL như minh họa trong Hình 2.

Hình 1 cho thấy trang **Create canary** trong **CloudWatch console**. Để sử dụng blueprint **Heartbeat monitoring** nhằm giám sát nhiều URL, hãy điền đầy đủ các trường (fields) như minh họa trong Hình 1. Sau khi nhập xong các thông tin cần thiết, nhấn nút Create canary ở cuối trang.

<div align="center">
  <img src="/images/3-Translates%20Blog/Blog%201/Figure1_Monitoring_multiple_URLs_in_heartbeat_monitoring_blueprint.png" width="70%" alt="Hình 1: Trang Create canary">
</div>

> **Hình 1: Trang Create canary**

Chọn canary từ [danh sách canary](https://console.aws.amazon.com/cloudwatch/home#synthetics:canary/list) và điều hướng đến trang chi tiết canary. Bạn sẽ thấy canary đang ở trạng thái **Running**. Nhấp vào tab **Availability** để xem thông tin về các lần chạy gần đây.

Hình 2 minh họa phần step summary trong báo cáo chạy canary trong CloudWatch console:

<div align="center">
  <img src="/images/3-Translates%20Blog/Blog%201/Figure2_Step_summary_-of_the_canary_run_report.png" width="80%" alt="Step Summary">
</div>

> **Hình 2 : Tóm tắt kết quả từng bước trong báo cáo chạy canary**

Nếu bạn đang giám sát nhiều URL bằng *Heartbeat monitoring blueprint*:

* Các canary sử dụng phương thức `executeStep()` hoặc `executeHttpStep()` từ thư viện Synthetics cũng sẽ xuất bản các chỉ số (metrics) **SuccessPercent** và **Duration**, với các chiều là **CanaryName** và **StepName** cho từng bước.
* Với các canary sử dụng `syn-nodejs-puppeteer-3.1` hoặc mới hơn, tùy chọn `setConfig` hỗ trợ nhiều tham số Boolean xác định những chỉ số nào được xuất bản.

Trong ví dụ sau, `setConfig` cho phép tất cả các bước tiếp tục chạy ngay cả khi một số bước thất bại. Nó cũng vô hiệu hóa việc chụp ảnh màn hình khi bắt đầu bước:

```javascript
syntheticsConfiguration.setConfig({
    continueOnStepFailure : true,
    screenshotOnStepStart : false
}); 
```
**Về tác giả**

| |
| :--- |
| **Shree Chinnasamy** <br><br> <img src="/images/3-Translates%20Blog/Blog%201/Shree-Chinnasamy-Profile.jpg" align="left" width="200px" style="margin-right: 25px; border-radius: 50%;"> <span style="font-size: 25px;">Shree Chinnasamy là Kiến trúc sư Giải pháp Chuyên gia Cao cấp trong nhóm Cloud Operations tại AWS. Anh tập trung chủ yếu vào các dịch vụ giám sát và khả năng quan sát (observability) của AWS như Amazon CloudWatch, AWS X-Ray, Amazon Managed Service for Prometheus và Amazon Managed Grafana. Anh có bằng Thạc sĩ Khoa học chuyên ngành Quản lý Hệ thống Viễn thông tại ĐH Northeastern, Boston. Là một người đam mê đọc sách và đã hoàn thành nhiều cuộc thi marathon, Shree hiện đang sinh sống tại bang Washington, khu vực Tây Bắc Thái Bình Dương. LinkedIn: www.linkedin.com/in/shreekarthic</span> |



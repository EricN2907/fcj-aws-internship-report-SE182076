---
title: "Blog 3"
date: 2025-09-09
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# Giới thiệu AWS Zero Trust Accelerator dành cho Chính phủ

**Tác giả:** Derek Doerr  

**Ngày đăng:** 6 tháng 5 năm 2025  

**Danh mục:** [Announcements](https://aws.amazon.com/blogs/security/category/post-types/announcements/), [Compliance](https://aws.amazon.com/blogs/security/category/security-identity-compliance/compliance/), [Foundational (100)](https://aws.amazon.com/blogs/security/category/learning-levels/foundational-100/), [Government](https://aws.amazon.com/blogs/security/category/public-sector/government/), [Public Sector](https://aws.amazon.com/blogs/security/category/public-sector/), [Security, Identity, & Compliance](https://aws.amazon.com/blogs/security/category/security-identity-compliance/)

---

Các cơ quan chính phủ đang đối mặt với thách thức chưa từng có trong việc thiết kế các biện pháp bảo mật chống truy cập trái phép vào hạ tầng công nghệ thông tin và dữ liệu. Các mô hình bảo mật truyền thống dựa trên ranh giới mạng — được xây dựng dựa trên giả định rằng mọi thành phần bên trong mạng nội bộ của tổ chức đều đáng tin cậy — nay không còn đủ để đảm bảo an toàn nữa. Việc phổ biến mô hình “mang thiết bị cá nhân” (BYOD - Bring Your Own Device) và sử dụng tài nguyên dựa trên đám mây (cloud-based resources) đã buộc các tổ chức phải áp dụng những biện pháp bảo mật bổ sung vượt ra ngoài mô hình truyền thống dựa trên ranh giới mạng. Những sự cố an ninh mạng quy mô lớn, như [khai thác lỗ hổng JetBrains (CVE) trên toàn cầu](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-347a) và [việc các nhóm tin tặc do chính phủ Iran hậu thuẫn tấn công mạng liên bang Mỹ](https://www.cisa.gov/news-events/cybersecurity-advisories/aa22-320a), đã cho thấy giới hạn của mô hình bảo mật truyền thống dựa trên ranh giới mạng.

Nhận thấy tính cấp bách của vấn đề, Chính quyền Tổng thống Biden đã ban hành Sắc lệnh [Hành pháp 14028](https://www.federalregister.gov/documents/2021/05/17/2021-10460/improving-the-nations-cybersecurity) – “Cải thiện an ninh mạng quốc gia” vào tháng 5 năm 2021. Sắc lệnh này yêu cầu các cơ quan liên bang Mỹ phải chuyển sang mô hình kiến trúc Zero Trust (ZTA) để tăng cường năng lực phòng vệ mạng và bảo vệ cơ sở hạ tầng trọng yếu khỏi các mối đe dọa mạng. Bên cạnh đó, Bộ Quốc phòng (DoD) và Cơ quan An ninh mạng và An toàn Hạ tầng (CISA) cũng đã công bố các hướng dẫn toàn diện về việc triển khai nguyên tắc Zero Trust, bao gồm: Chiến lược Zero Trust của Bộ Quốc phòng ([DoD Zero Trust Strategy](https://dodcio.defense.gov/Portals/0/Documents/Library/DoD-ZTStrategy.pdf)) và Mô hình trưởng thành Zero Trust của CISA ([CISA Zero Trust Maturity Model](https://www.cisa.gov/sites/default/files/2023-04/CISA_Zero_Trust_Maturity_Model_Version_2_508c.pdf))

Văn phòng Quản lý và Ngân sách Hoa Kỳ (OMB) đã đặt ra mục tiêu cho các cơ quan hành pháp dân sự liên bang (FCEB) thực hiện các hướng dẫn của CISA trong năm tài chính (FY) 2024 và 2025, trong khi Bộ Quốc phòng (DoD) đặt mục tiêu cho năm tài chính (FY) 2027 và các năm tiếp theo.

Nguyên tắc Zero Trust tập trung vào việc cấp quyền truy cập tới các tài nguyên được bảo vệ như dữ liệu, ứng dụng, và dịch vụ dựa trên việc xác minh liên tục danh tính và hiện trạng bảo mật (security posture) của mọi người dùng, thiết bị, và giao dịch, bất kể vị trí mạng. Cách tiếp cận này nhằm loại bỏ khái niệm “tin cậy ngầm định” (implicit trust), đảm bảo rằng chỉ các thực thể đã được xác thực mới có quyền truy cập vào tài nguyên nhạy cảm, đồng thời giảm thiểu rủi ro truy cập trái phép và di chuyển ngang trong hệ thống mạng.

[Amazon Web Services (AWS)](https://aws.amazon.com/) đang đi đầu trong sự chuyển đổi mô hình bảo mật này, cung cấp bộ giải pháp và năng lực chuyên biệt cho khu vực chính phủ, giúp các cơ quan chuyển đổi sang mô hình Zero Trust một cách hiệu quả. Cách tiếp cận Zero Trust được AWS khuyến nghị được thiết kế để cung cấp một chiến lược an ninh mạng (cybersecurity strategy) mạnh mẽ, có khả năng mở rộng và hướng tới tương lai, vốn phù hợp với các yêu cầu (và chỉ thị) của chính phủ, đồng thời trao quyền (hoặc giúp) các cơ quan bảo vệ hiệu quả các tài nguyên quan trọng trong sứ mệnh của mình.

## **Cách tiếp cận ZTAG của AWS: Giải pháp tập trung cho khu vực chính phủ**

[AWS Zero Trust Accelerator for Government (ZTAG)](https://aws.amazon.com/government-education/government/mission-innovation-solutions/) là một bộ tài nguyên được thiết kế riêng cho các tổ chức chính phủ nhằm hỗ trợ triển khai kiến trúc Zero Trust. ZTAG bao gồm nhiều công cụ tăng tốc khác nhau, chẳng hạn như:

* Công cụ đánh giá mức độ trưởng thành về Zero Trust
* Kiến trúc tham chiếu và hướng dẫn triển khai
* Tích hợp các dịch vụ AWS và giải pháp từ các đối tác phần mềm độc lập (ISV) của AWS
* Các mẫu triển khai tham chiếu của AWS ISV hợp tác cùng các đối tác ISV hàng đầu trong ngành
* Quy trình mua sắm được tinh giản thông qua **AWS Marketplace**

Các công cụ đánh giá trong ZTAG giúp bạn xác định khoảng cách giữa hiện trạng và các yêu cầu Zero Trust của chính phủ, đồng thời cung cấp hướng dẫn và khuyến nghị phù hợp (tailored). Bộ công cụ này bao gồm các dịch vụ AWS và giải pháp từ các đối tác ISV được thiết kế để hỗ trợ bạn thực hiện các hoạt động cụ thể theo khung Zero Trust của Bộ Quốc phòng Hoa Kỳ (DoD) hoặc các chức năng Zero Trust của CISA. Ban đầu, ZTAG tập trung vào các khung Zero Trust của chính phủ Hoa Kỳ, có thể áp dụng ở cấp liên bang, bang và địa phương, và đã có lộ trình mở rộng để bao gồm các khung Zero Trust quốc tế.

## **Thúc đẩy việc áp dụng Zero Trust cùng AWS**

Cách tiếp cận ZTAG được thiết kế đặc biệt để đáp ứng các yêu cầu và thách thức riêng của các cơ quan chính phủ, mang lại nhiều lợi ích nổi bật:

* Phù hợp với các mô hình Zero Trust của DoD và CISA, đồng thời có khả năng mở rộng cho các mô hình của chính phủ hoặc ngành khác khi chúng xuất hiện (as they emerge).
* Tăng tốc lộ trình xây dựng hạ tầng CNTT an toàn và có khả năng phục hồi (resilient), giúp xác định khoảng cách Zero Trust và xây dựng lộ trình đạt được mục tiêu an ninh mạng.
* Dựa trên năng lực hiện có của cơ quan bạn, đồng thời mở rộng bằng các giải pháp tối ưu từ các đối tác ISV hàng đầu của AWS.
* Phương pháp tiếp cận gia tăng (Incremental approach) giúp chuyển đổi sang kiến trúc Zero Trust một cách mượt mà (smooth).
* Đội ngũ chuyên gia chuyên biệt hỗ trợ các cơ quan chính phủ trong suốt hành trình triển khai Zero Trust.

## **Bắt đầu với ZTAG**

Để bắt đầu hành trình Zero Trust, các cơ quan chính phủ có thể sử dụng các công cụ đánh giá Zero Trust của AWS, được điều chỉnh phù hợp với các khung DoD hoặc CISA. Hãy làm việc với một chuyên gia Zero Trust chuyên biệt (dedicated zero trust specialist) để hoàn thành đánh giá môi trường hiện tại của bạn. Các bản đánh giá này giúp xác định mức độ trưởng thành Zero Trust hiện tại, chỉ ra chính xác (pinpoint) các khoảng cách (gaps) và phát triển lộ trình tùy chỉnh phù hợp với yêu cầu và ngân sách cụ thể của cơ quan. Bạn có thể đánh giá lại môi trường bất kỳ lúc nào để theo dõi tiến trình theo thời gian.

<div align="center">
  <img src="/images/3-Translates Blog/Blog 3/AWS-Zero-Trust-Accelerator-1.png" width="70%" alt="">
</div>

**Hình 1:** Ví dụ về các giai đoạn trưởng thành theo trụ cột của DoD

<div align="center">
  <img src="/images/3-Translates Blog/Blog 3/AWS-Zero-Trust-Accelerator-2.png" width="70%" alt="">
</div>

**Hình 2:** Ví dụ về các hoạt động theo mức độ trưởng thành của DoD

![]()



## **Kết luận**

AWS Zero Trust Accelerator for Government (ZTAG) thể hiện cam kết của AWS trong việc hỗ trợ các cơ quan liên bang Hoa Kỳ chuyển đổi sang kiến trúc Zero Trust. Bằng cách kết hợp cơ sở hạ tầng đám mây AWS với các giải pháp bảo mật hàng đầu trong ngành, ZTAG mang đến một cách tiếp cận linh hoạt, tập trung cho chính phủ để xây dựng hiện trạng an ninh mạng vững chắc mà vẫn duy trì được tính linh hoạt trong vận hành.

Các cơ quan chính phủ có thể sử dụng ZTAG để tăng tốc độ áp dụng Zero Trust, nâng cao năng lực an ninh tổng thể và đáp ứng các yêu cầu tuân thủ quan trọng.
 Liên hệ với nhóm tài khoản AWS của bạn để tìm hiểu thêm về cách AWS có thể hỗ trợ hành trình Zero Trust của cơ quan bạn.

Nếu bạn có phản hồi về bài đăng này, hãy gửi bình luận trong phần Comments (Bình luận) bên dưới.

**Về tác giả**

| |
| :--- |
| **Derek Doerr** <br><br> <img src="/images/3-Translates%20Blog/Blog%203/Derek-Doerr.jpg" align="left" width="200px" style="margin-right: 25px; border-radius: 50%;"> <span style="font-size: 25px;">Derek Doerr là một lãnh đạo công nghệ cấp cao và Trưởng nhóm chuyên trách Zero Trust (Zero Trust Single-Threaded Leader) cho khu vực AWS US Federal, với chuyên môn trong chiến lược bảo mật và quản trị đám mây (cloud governance). Với hơn 30 năm kinh nghiệm trong cả khu vực tư nhân và công, ông dẫn dắt các sáng kiến chiến lược và duy trì văn hóa bảo mật trong tổ chức. Ngoài công việc, Derek yêu thích dành thời gian cho gia đình, nấu ăn, lặn biển (scuba diving) và du lịch.</span> |
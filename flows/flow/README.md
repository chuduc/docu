---
description: Xây dựng kịch bản tự động cho bạn và doanh nghiệp
---

# Flow

### &#x20;Flow là gì?

Flow là kịch bản được thiết kế sẵn cho phép bạn tự động hoá quy trình công việc và giao tiếp với khách hàng.  Flow hoạt động với chung một nguyên tắc: "Khi sự kiện này xảy ra, thực hiện hành động này".

Kịch bản này hoàn toàn tự động và được kích hoạt bởi một hoặc nhiều Trigger từ các nền tảng khác nhau, cùng thực hiện chung 1 quy trình giao tiếp/ hành động.

Trong LadiFlow có 3 loại Flow:

* **One Channel Flow**: là một chuỗi tin nhắn trên 1 kênh duy nhất. Ví dụ Email, Messenger..
* **Cross-Channel flow**: Là một chuỗi các tin nhắn trên nhiều kênh khác nhau. Ví dụ gồm hai email, một tin nhắn Messenger, một tin nhắn Zalo
*   **Multi-Flow**: là một Flow kết nối các Flow khác nhau thành một Flow mới với nhiều điều kiện khác nhau\


    <figure><img src="../../.gitbook/assets/image (569).png" alt=""><figcaption><p>Một số kịch bản mẫu</p></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (681).png" alt=""><figcaption><p>Kịch bản gửi Email, SMS chúc mừng sinh nhật</p></figcaption></figure>

Một Flow trong LadiFlow gồm các thành phần sau:

* **Tên Flow**
* **Tags của Flow**
* **Triggers**
* **Actions**

**Tags** của Flow giúp bạn dễ dàng quản lý quản lý Flow theo Tags (thẻ).

**Trigger** là sự kiện sẽ kích hoạt Flow. Flow trên LadiFlow cho phép nhiều Trigger thực hiện cùng một chuỗi hành động. Các sự kiện kích hoạt có thể từ chính trên LadiFlow hoặc các nền tảng khác: Facebook, Zalo, LadiChat, LadiSales....

**Ví dụ:**&#x20;

* Sự kiện khách hàng bình luận bài viết trên Facebook Page
* Sự kiện khách hàng quan tâm Zalo OA
* Sự kiện khi có đơn hàng mới được tạo trên LadiSales

**Actions** là chuỗi các hành động trong một quy trình có thứ tự. Khi có Trigger (sự kiện), hành động đầu tiên trong chuỗi sẽ thực hiện. Các hành động này sẽ thực hiện trên khách hàng kích hoạt trigger đó. **Tỷ lệ thực hiện hành động thành công phụ thuộc vào tập dữ liệu khách hàng của bạn.**

**Ví dụ**&#x20;

* Tập khách hàng của bạn tương tác qua Facebook thì bạn nên thực hiện các hành động của LadiFlow và Messenger.
* Tập khách hàng của bạn tương tác qua LadiPage/Website thì bạn nên thực hiện hành động gửi Email với điều kiện "Xác thực Email" là "Đã xác thực".

{% hint style="info" %}
Bạn nên tạo trigger tương ứng nền tảng với hành động để tăng tỷ lệ thực hiện hành động thành công.
{% endhint %}

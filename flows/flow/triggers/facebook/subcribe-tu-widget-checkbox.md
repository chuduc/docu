---
description: >-
  Sự kiện Khách hàng tích chọn vào checkbox nhắn tin với Page trên website của
  bạn
---

# Subcribe từ Widget checkbox

Trigger hoạt động khi có người click vào checkbox tiện ích của Facebook trên website của bạn. Tính năng này tương tự như Subcribe từ Widget Button nhưng với giao diện là checkbox. Khách hàng sau khi click vào checkbox sẽ được điều hướng sang màn hình nhắn tin với Page Facebook.

<figure><img src="../../../../.gitbook/assets/image (596).png" alt=""><figcaption></figcaption></figure>

**Lưu ý:**

* Chỉ thực hiện được khi website được nhúng mã nhúng của LadiFlow và  gắn checkbox của LadiFlow đúng vị trí.
* Chỉ thực hiện các hành động trong Flow với những ai tích chọn vào checkbox tiện ích và đăng nhập thành công Messenger.
* Hệ thống sẽ tự động tạo khách hàng mới nếu tập khách hàng của bạn chưa có dữ liệu của khách hàng này.

1.  Chọn **+Thêm Trigger,** tìm và **chọn Subcribe từ Widget Checkbox** .\


    <figure><img src="../../../../.gitbook/assets/image (538).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Chọn tài khoản Facebook cấu hình**. Nếu bạn chưa có hãy tích hợp thêm.
3. Mở mục Thiết lập trigger, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4.  **Chỉnh sửa vị trí và kích thước của checkbox**, hệ thống sẽ hiển thị preview tương ứng.\


    <figure><img src="../../../../.gitbook/assets/image (699).png" alt="" width="419"><figcaption></figcaption></figure>

    Xem trước hình ảnh widget tại đây

<figure><img src="../../../../.gitbook/assets/image (700).png" alt="" width="422"><figcaption></figcaption></figure>

2. **Copy mã nhúng và nhúng vào website của bạn.**
3. **Chọn kiểm tra tài khoản Page Facebook** để chắc chắn rằng tài khoản page của bạn vẫn đang hoạt động.

**Lưu ý**:&#x20;

* Trigger chỉ có thể hoạt động khi website của bạn có mã nhúng của trigger LadiFlow.
* Mã nhúng phải được nhúng vào đúng vị trí.

**Gợi ý các hành động phù hợp với Trigger:**

* **Gửi tin nhắn Messenger**
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....

### Gắn SDK và checkbox vào Landing Page/Website của bạn trên LandiPage

**Thêm SDK**

1. Mở chi tiết landing page của bạn trên LadiPage
2. Chọn Mã JavaScript/CSS

<figure><img src="../../../../.gitbook/assets/image (570).png" alt="" width="248"><figcaption></figcaption></figure>

3. Sao chép SDK trong chi tiết Trigger&#x20;

<figure><img src="../../../../.gitbook/assets/image (571).png" alt=""><figcaption></figcaption></figure>

4. Dán vào mục Trước thẻ \</head> trên LadiPage

<figure><img src="../../../../.gitbook/assets/image (572).png" alt="" width="375"><figcaption></figcaption></figure>

5. Sao chép Mã nhúng button trong chi tiết Trigger trên LadiFlow

<figure><img src="../../../../.gitbook/assets/image (573).png" alt=""><figcaption></figcaption></figure>

6. Thêm phần tử Mã HTML vào landing page

<figure><img src="../../../../.gitbook/assets/image (575).png" alt=""><figcaption></figcaption></figure>

7. Chọn Sửa HTML

<figure><img src="../../../../.gitbook/assets/image (695).png" alt=""><figcaption></figcaption></figure>

8. Dán mã nhúng button đã sao chép vào biểu mẫu Chỉnh sửa HTML

&#x20;

<figure><img src="../../../../.gitbook/assets/image (696).png" alt="" width="563"><figcaption></figcaption></figure>

9. Xuất bản landing page để xem và kiểm tra sdk và checkbox vừa gắn.

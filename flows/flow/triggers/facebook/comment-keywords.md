---
description: Sự kiện khi khách hàng bình luận vào 1 bài viết trên Page Facebook của bạn
---

# Comment Keywords

Trigger hoạt động khi có ai đó bình luận vào bài viết trên page Facebook của bạn. Bạn có thể tuỳ chỉnh bài viết cụ thể hoặc tất cả các bài viết. Ngoài ra bạn cũng có thể tuỳ chỉnh trigger hoạt động với điều kiện bình luận chứa hoặc không chứa từ khoá cụ thể.

### Thiết lập trigger Facebook Comment Keywords

1.  Chọn **+Thêm Trigger,** tìm và chọn Trigger **Facebook Comment Keywords.**\


    <figure><img src="../../../../.gitbook/assets/image (540).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2.  **Chọn tài khoản Facebook** cấu hình trigger .\


    <figure><img src="../../../../.gitbook/assets/image (706).png" alt="" width="425"><figcaption></figcaption></figure>
3. Chọn mục Thiết lập trigger, thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong Flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Chọn bài viết cụ thể Trigger sẽ hoạt động hoặc tất cả bài viết.**

<figure><img src="../../../../.gitbook/assets/image (522).png" alt=""><figcaption></figcaption></figure>

Nếu chọn Một bài viết cụ thể, bạn phải chọn bài viết kích hoạt Trigger:

* Chọn bài đăng trên Trang Facebook: **Chọn bài đăng từ tab** "**Danh sách bài đăng"** hoặc bằng cách **nhập** **ID bài đăng trong tab "Tùy chọn"**.

<figure><img src="../../../../.gitbook/assets/image (39).png" alt="" width="563"><figcaption><p>Tab Danh sách bài đăng</p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (50).png" alt="" width="563"><figcaption><p>Tab Tùy chọn</p></figcaption></figure>

* Bạn có thể xem chi tiết bài viết bằng cách chọn Xem bài đăng.
* Bạn cũng có thể đổi sang bài viết khác sau khi đã chọn 1 bài viết.\


<figure><img src="../../../../.gitbook/assets/image (52).png" alt="" width="563"><figcaption></figcaption></figure>

5.  **Chọn điều kiện bình luận:** bình luận chứa từ khoá cụ thể, bình luận chứa từ khoá bất kỳ.

    Nếu chọn bình luận chứa từ khoá cụ thể, bạn hãy nhập từ khoá, sau đó nhấn enter để thêm từ khoá như hình dưới đây

<figure><img src="../../../../.gitbook/assets/nhập từ khóa fb (1).gif" alt="" width="462"><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (566).png" alt=""><figcaption></figcaption></figure>

5.  Bật/ tắt lựa chọn Chỉ áp dụng cho cấp đầu tiên.

    Nếu bạn bật, hệ thống chỉ kiểm tra các bình luận cấp đầu tiên, ngược lại hệ thống kiểm tra tất cả các cấp của bình luận.
6.  Bật/Tắt kích hoạt trigger khi người dùng bình luận Email hoặc số điện thoại.

    Nếu bật các bình luận có chứa email hoặc số điện thoại sẽ kích hoạt trigger và ngược lại nếu tắt trigger sẽ hoạt động như phần cài đặt ở trên.
7. Chọn lưu lại thông tin email, số điện thoại nếu muốn lưu email và số điện thoại khách hàng nếu khách hàng bình luận có chứa email và số điện thoại.
8.  &#x20;**Chọn +Thêm bình luận nếu muốn điền nội dung bình luận phản hồi tại bình luận của khách hàng**. Sau đó nhập nội dung mong muốn. LadiFlow cho phép bạn nhập nhiều bình luận phản hồi.\


    <figure><img src="../../../../.gitbook/assets/image (708).png" alt="" width="418"><figcaption></figcaption></figure>
9. Chọn tự động thích, ẩn bình luận của khách hàng nếu muốn.
10. **Kiểm tra tài khoản Facebook** để chắc chắn Trigger sẽ hoạt độn&#x67;**.**

{% hint style="info" %}
**Lưu ý:**&#x20;

* Khi có bất kỳ ai bình luận vào bài viết của bạn, 1 khách hàng trên LadiFlow sẽ tự động được tạo mới nếu chưa có dữ liệu về khách hàng đó.
* Nếu bạn muốn gửi tin nhắn Messenger khi khách bình luận vào bài viết thì hành động Gửi tin Messenger bắt buộc phải là hành động đầu tiên của Flow
* Do quy định của Facebook, tin nhắn gửi tự động khi khách bình luận chỉ được 1 nội dung: tin nhắn kèm nút hoặc hình ảnh hoặc file hoặc bộ sưu tập... Nếu bạn thiết lập nhiều hơn 1 nội dung trong tin nhắn đầu tiên của Flow, các nội dung khác sẽ gửi thất bại.
{% endhint %}

**Gợi ý các hành động phù hợp với Trigger:**

* **Gửi tin nhắn Messenger( phải là hành động đầu tiên trong Flow)**
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....

### Cách lấy ID bài đăng trên Facebook Page

1. Truy cập [Meta Business Suite](https://business.facebook.com/).
2. Vào mục **Nội dung** > chọn tab **Bài viết & Thước phim.**

<figure><img src="../../../../.gitbook/assets/image (45).png" alt="" width="563"><figcaption></figcaption></figure>

3. Tìm bài đăng mà bạn muốn, bấm vào bài đăng để xem chi tiết bài đăng và sao chép ID bài đăng.

<figure><img src="../../../../.gitbook/assets/image (46).png" alt="" width="563"><figcaption></figcaption></figure>

**Với những bài đăng dạng Thước phim:**  Tại danh sách Bài viết & Thước phim, bấm vào thước phim mà bạn muốn -> Chuyển hướng đến trang chi tiết -> Nhấn vào nút Sao chép ID bài viết.

<figure><img src="../../../../.gitbook/assets/image (47).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (48).png" alt="" width="563"><figcaption></figcaption></figure>

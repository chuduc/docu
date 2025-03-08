---
description: Sự kiện Khách hàng quét QR hoặc truy cập m.me link
---

# Subscribe từ m.me link

Trigger hoạt động khi có người click vào đường dẫn m.me hoặc quét mã QR. m.me là dịch vụ URL do Meta cung cấp nhằm chuyển hướng người dùng đến một người, trang hoặc cuộc trò chuyện trên Messenger.

Đường dẫn m.me LadiFlow tự động tạo theo tài khoản bạn cấu hình.

1. Chọn **+ Thêm trigger**, sau đó tìm và chọn **Đường dẫn theo dõi từ m.me link.**

<figure><img src="https://lh5.googleusercontent.com/5P_aOM6RcF8yGRoZaB8wvUjRxpkreIZqhXNtF-sw6bygFByXaKf1TNMOSuvKD79_Oko3hMtNwTWOfr06Xc68x4ge8v5QyQh9f8eTNCEKgJfw3DiTaSBB0DqmzdfGVD3IyG2GQzE1y52sppcdgpxvGhE" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2.  **Chọn tài khoản Facebook cấu hình**. Nếu chưa có tài khoản hãy tích hợp thêm, xem hướng dẫn tại [https://help.ladiflow.vn/tich-hop/huong-dan-tich-hop](https://help.ladiflow.vn/tich-hop/huong-dan-tich-hop)\


    <figure><img src="../../../../.gitbook/assets/image (697).png" alt="" width="424"><figcaption></figcaption></figure>
3. Mở mục Thiết lập trigger chọn Điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong Flow xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4.  &#x20;**Copy đường dẫn hoặc tải xuống QR** để khách hàng của bạn truy cập.\


    <figure><img src="../../../../.gitbook/assets/image (698).png" alt="" width="426"><figcaption></figcaption></figure>
5. **Chọn kiểm tra tài khoản Page Facebook** để chắc chắn rằng tài khoản page của bạn vẫn đang hoạt động.

{% hint style="info" %}
**Lưu ý:**&#x20;

* Khi một người nhấp vào liên kết m.me, người đó sẽ được chuyển hướng đến cuộc trò chuyện mới với Page của bạn hoặc cuộc trò chuyện hiện có nếu người đó từng nhắn tin cho Page. Cuộc trò chuyện này sẽ hiển thị một tin nhắn mặc định có nội dung "Bạn đã tham gia cuộc trò chuyện này thông qua một liên kết. Chúng tôi đã cho PAGE-NAME biết bạn đang ở đây."
* Khi có 1 người click vào link hoặc quét QR, hệ thống tự động tạo 1 khách hàng trên LadiFlow nếu đó là khách hàng mới.
* Nếu khách hàng lần đầu nhắn tin với Page, Facebook sẽ hiện nút Bắt đầu. Khách hàng phải nhấn Bắt đầu thì các tin nhắn thiết lập trong kịch bản sẽ được gửi. Nút Bắt đầu là quy định của Facebook, được coi như hành động đồng ý Page gửi tin nhắn cho khách hàng.
{% endhint %}

**Gợi ý các hành động phù hợp với Trigger:**

* **Gửi tin nhắn Messenger**
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....

### Gắn tham số vào link mme&#x20;

Khi bạn muốn khách hàng hoàn thành form trên LadiPage gửi tin nhắn chứa nội dung khách hàng đã nhập trên form bạn làm như sau:

1. Thêm các tham số vào link m.me mà bạn điền vào URL cảm ơn hoặc link mở trên ứng dụng mobile theo format như sau

\<Link m.me từ trigger trên LadiFlow>|\<Tên trường tùy chỉnh LadiFlow>:\{{Tên trường tùy chỉnh trên form LadiPage\}}

Ví dụ:

[https://m.me/198695534010449?ref=732c85a41f93baa7|full\_name:\{{name\}}|email:\{{email\}}|phone:\{{phone\}}](https://m.me/198695534010449?ref=732c85a41f93baa7|name:\{{name\}}|email:\{{email\}}|phone:\{{phone\}}|text:\{{message\}})

<figure><img src="../../../../.gitbook/assets/image (289).png" alt="" width="375"><figcaption><p>Tên trường tùy chỉnh LadiPage</p></figcaption></figure>

2. Quay trở lại Flow có trigger click vào m.me link, bạn có thể tủy chỉnh tin nhắn Messenger có các thông tin trường tùy chỉnh của khách hàng theo các dữ liệu đã gắn từ Form

<figure><img src="../../../../.gitbook/assets/image (291).png" alt="" width="563"><figcaption></figcaption></figure>

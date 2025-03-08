# Báo cáo Flow

Báo cáo chi tiết các thông tin của Flow, báo cáo chi tiết từng hành động trong Flow và từng khách hàng thực hiện trong Flow.

1. **Chọn Flow muốn xem báo cáo.**
2.  **Chọn Xem báo cáo .**\


    <figure><img src="../.gitbook/assets/image (560).png" alt=""><figcaption></figcaption></figure>

LadiFlow giúp bạn có thể xem báo cáo chi tiết từng hành động trong flow: tỷ lệ mở, tỷ lệ click, số lượt gửi....

<figure><img src="../.gitbook/assets/image (751).png" alt="" width="563"><figcaption></figcaption></figure>

Để xem chi tiết báo cáo từng Trigger và khoảng thời gian, chọn bộ lọc ở đây.\


<figure><img src="../.gitbook/assets/image (752).png" alt="" width="563"><figcaption></figcaption></figure>

### Giải thích các số liệu trong báo cáo

#### Tổng lượt chạy

Lượt chạy là số lần thực hiện trên tất cả Trigger trong Flow.

<figure><img src="../.gitbook/assets/image (762).png" alt="" width="563"><figcaption></figcaption></figure>

#### Doanh thu

Doanh thu được đo lường bằng tổng giá trị đơn hàng mà khách hàng click từ link trong email và thực hiện tạo đơn. Email chứa link bán hàng trong Flow nào thì doanh thu được tính cho Flow đó.

<figure><img src="../.gitbook/assets/image (763).png" alt="" width="563"><figcaption></figcaption></figure>

**Tổng số lượt thực hiện hành động và tỷ lệ thực hiện hành động**\


<figure><img src="../.gitbook/assets/image (318).png" alt="" width="347"><figcaption></figcaption></figure>

**Tổng số lượt thực hiện hành động**: tổng số lượt đã/được thực hiện hành động mà người đó thoả mãn điều kiện kích hoạt trigger.&#x20;

**Tỷ lệ thực hiện hành động=Tổng số lượt thực hiện hành động /Tổng số lượt thực hiện trigger**

### Lượt nhận&#x20;

<figure><img src="../.gitbook/assets/image (764).png" alt="" width="374"><figcaption></figcaption></figure>

**Số lượt nhận =** số lượt thực hiện hành động thành công

Ví dụ: các hành động gửi email, tin nhắn thì đây là số lượt email đã gửi thành công, tin nhắn thành công. Nếu hành động gọi AI call thì đây là số lượt nhận được cuộc gọi.

### Tỷ lệ mở và số lượt hàng mở

<figure><img src="../.gitbook/assets/image (319).png" alt=""><figcaption></figcaption></figure>

**Số lượt mở** = số lượt mở tin nhắn, email trong flow. Lượt mở chỉ được ghi nhận 1 lần nếu khách hàng mở tin nhiều lần. Với các hành động không phải gửi email, tin nhắn số khách hàng mở =0.

**Tỷ lệ mở= số lượt mở/Tổng số lượt kích hoạt trigger.**

### Tỷ lệ click và số lượt click

<figure><img src="../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

**Số lượt click**= số lượt click khác nhau click vào link, nút.. có trong nội dung tin nhắn, email đó. Với các hành động không phải gửi email, tin nhắn và nội dung email, tin nhắn không có link, nút thì số lượt click =0.

**Tỷ lệ click= số lượt click/Tổng số lượt thực hiện hành động**

{% hint style="info" %}
**Với các tin nhắn không chứa link, nút tỷ lệ click =0 và số lượt click =0.**

**Với các hành động không phải email, tin nhắn, số lượt mở và số lượt click =0.**
{% endhint %}

### Báo cáo chi tiết từng hành động

Bạn chọn vào hành động muốn xem báo cáo, báo cáo sẽ hiển thị thông tin bên cạnh.\


<figure><img src="../.gitbook/assets/image (765).png" alt="" width="432"><figcaption></figcaption></figure>

Tuỳ theo từng hành động, LadiFlow cung cấp cho bạn những chỉ số báo cáo khác nhau. Những chỉ số này tính theo lượt hành động của khách hàng và hệ thống.&#x20;

* **Đã gửi:** số request LadiFlow đã gửi yêu cầu thực hiện hành động.
* **Đã nhận**: số tin nhắn/hành động được thực hiện thành công.
* **Đã mở**: số tin nhắn/email khách hàng đã mở.
* **Đã click**: tổng số click trên các tin nhắn/email nếu chưa link, nút.
* **Đã hủy đăng ký**: tổng số lượt hủy đăng ký ( đối với email).
* **Đã báo xấu**: số email bị báo xấu.
* **Bị trả về:** số email bị trả về(bounces).

Với các hành động với bên thứ 3 (Email, Zalo, Messenger, AI call....) tỷ lệ thành công phụ thuộc vào bên thứ 3, chất lượng dữ liệu và khách hàng của bạn. Ví dụ bạn gửi tin nhắn Messenger cho khách hàng khi khách hàng bình luận vào bài viết của bạn, khách hàng chặn page của bạn, tắt mạng, khoá tài khoản hoặc Messenger gửi tin không thành công do Page của bạn bị khoá... thì sẽ không thể thực hiện hành động thành công được. Ngoài ra lựa chọn hành động không phù hợp cũng dẫn tới tỷ lệ thành công thấp ví dụ tập khách hàng của bạn lấy từ Facebook nhưng bạn gửi email khi chưa có đủ thông tin email của họ.&#x20;

#### Xem danh sách khách hàng trong hành động

Bạn chọn Danh sách khách hàng chi tiết để xem danh sách khách hàng trong hành động đó.\


<figure><img src="../.gitbook/assets/image (766).png" alt="" width="424"><figcaption></figcaption></figure>

Bạn sẽ xem được chi tiết từng khách hàng tương tác với thông điệp của bạn: trạng thái, lượt mở, lượt click.\


<figure><img src="../.gitbook/assets/image (768).png" alt="" width="563"><figcaption></figcaption></figure>

Danh sách đã được gom nhóm theo ngày, số lượt tương tác là số lần tương tác của khách hàng theo trạng thái bạn chọn. \
Ví dụ bạn chọn Đã gửi, lượt tương tác của 1 khách hàng vào ngày 5/6/2024 là 2. Nghĩa là khách hàng vào ngày 5/6/2024 đã được vào Flow và thực hiện hành động 2 lần.

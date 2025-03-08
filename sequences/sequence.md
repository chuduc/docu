---
description: Là một chuỗi các tin nhắn tự động gửi đến khách hàng theo trình tự.
---

# Sequence

### Sequence là gì?

Sequence là một danh sách các tin nhắn được kích hoạt “có trình tự” để gửi tự động đến những người đăng ký mới, dựa trên mục đích của một chiến dịch Marketing.

Sequence trên LadiFlow cho phép bạn gửi chuỗi tin nhắn chăm sóc khách hàng theo thời gian được thiết lập.

Khi một ai đó đăng ký vào sequence thì họ sẽ lần lượt nhận được các thông điệp được thiết lập theo thời gian thiết lập.

LadiFlow cho phép bạn tạo Sequence với các tin nhắn qua các kênh khác nhau:

* Email
* SMS
* Zalo ZNS
* &#x20;ZALO quan tâm
* &#x20;AI Call
* Messenger

### Thiết lập 1 sequence

1. Chọn Sequences trên thanh menu bên trái, sau đó chọn Tạo Sequence.

<figure><img src="../.gitbook/assets/tạo sequence.png" alt=""><figcaption></figcaption></figure>

2. **Điền thông tin tên Sequence** và Tag (nếu có). Tên Sequence không được trùng với các Sequence bạn đã có.
3. **Chọn kênh gửi tin nhắn đầu tiên**: sms, email, mesenger, zalo .....
4. Nhập các thông tin thiết lập tin nhắn bạn vừa chọn. Bạn có thể tham khảo hướng dẫn nhập các thông tin tại [kenh-tin-nhan](../campaigns/kenh-tin-nhan/ "mention").

{% hint style="info" %}
Các dữ liệu bạn nhập sẽ được tự động lưu.
{% endhint %}

5. Chọn **Xuất bản hoặc Đóng**. Hệ thống tự động lưu nháp các thông tin bạn chỉnh sửa trong nội dung tin nhắn.
6. T**hêm các tin nhắn khác** vào trong Sequence và lặp lại cho đến khi đủ các tin nhắn trong Sequence.
7. **Thiết lập thời gian gửi cho từng tin nhắn.**

<figure><img src="../.gitbook/assets/image (884).png" alt=""><figcaption></figcaption></figure>

Bạn có thể thiết lập chi tiết khoảng thời gian sẽ gửi tin nhắn và tuỳ chọn thời gian gửi tin nhắn trong tuần:

* Chọn Gửi ngay để gửi ngay khi kích hoạt hoặc tin nhắn trước đó được gửi
* Chọn Khoảng thời gian để cài đặt thời gian nhận tin nhắn.&#x20;
* Chọn Mọi ngày để thay đổi ngày gửi tin nhắn trong tuần.

Nếu theo lịch tin nhắn của bạn gửi ngoài thời gian gửi tin đã thiết lập, khi đến thời gian thoả mãn tiếp theo, tin nhắn đó sẽ được gửi.

<figure><img src="../.gitbook/assets/setup delay sequence.gif" alt=""><figcaption></figcaption></figure>

8. **Kích hoạt** lần lượt các tin nhắn mong muốn

<figure><img src="../.gitbook/assets/image (883).png" alt=""><figcaption></figcaption></figure>

**Lưu ý**:&#x20;

* Hệ thống chỉ gửi những tin nhắn được kích hoạt. Các tin nhắn sẽ được gửi theo thời gian thiết lập của nó theo thứ tự từ trên xuống dưới. Thời điểm gửi tin sẽ được tính theo thời điểm tin nhắn gần nhất được xuất bản đã gửi( nếu là tin thứ 2 trở lên), và theo thời điểm đăng ký sequence (nếu là tin nhắn đầu tiên)

Ví dụ: bạn cài đặt theo thứ tự sau:

&#x20;Tin nhắn 1: gửi ngay sau 1 giờ, đã kích hoạt.

Tin nhắn 2: gửi sau 1 giờ, chưa kích hoạt.

Tin nhắn 3: gửi sau 2 giờ, đã kích hoạt.

->  1 tiếng sau khi khách hàng đăng ký sequence sẽ nhận được tin nhắn 1, sau khi tin nhắn 1 được gửi 2 giờ sẽ nhận được tin nhắn 3 (sau 3 giờ kể từ thời điểm đăng ký sequence).

* Chỉ khi khách hàng đăng ký Sequence, Sequence mới chạy với khách hàng đó.
* Nếu cho phép Sequence lặp lại, đăng ký lại Sequence với khách đã/đang chạy Sequence thì sau khi kết thúc Sequence sẽ thực hiện lại với khách hàng đó.

<figure><img src="../.gitbook/assets/image (888).png" alt=""><figcaption></figcaption></figure>

### Nhân bản Sequence

Chọn sequence muốn nhân bản, sau đó chọn Nhân bản

<figure><img src="../.gitbook/assets/image (307).png" alt=""><figcaption></figcaption></figure>

Hệ thống sẽ tạo ra 1 sequence mới có nội dung giống Sequence cũ, bạn có thể chỉnh sửa dữ liệu, xuất bản và kích hoạt tin nhắn.

**Lưu ý**:&#x20;

* Tất cả các tin nhắn trong Sequence nhân bản đều ở trạng thái chưa xuất bản. Với các tin nhắn bắt đầu Flow khác, Sequence nhân bản cũng nhân bản các Flow đó. Flow nhân bản này ở trạng thái Nháp.
* Để xuất bản tin nhắn, đảm bảo Flow bạn chọn trong tin nhắn (nếu có) đã xuất bản.

### Nhân bản tin nhắn trong Sequence

1. Di chuyển con trỏ chuột vào tin nhắn muốn nhân bản
2. Chọn **Nhân bản**

<figure><img src="../.gitbook/assets/image (585).png" alt=""><figcaption></figcaption></figure>

**Lưu ý:**&#x20;

* Với tin nhắn có gắn sang Flow khác, hệ thống cũng nhân bản Flow đó.
* Tin nhắn nhân bản được xếp vị trí cuối cùng trong Sequence.
* Trước khi xuất bản tin nhắn nhân bản, kiểm tra lại Flow đã gắn trong tin nhắn, đảm bảo Flow đó đã xuất bản.

### Đăng ký Sequence cho khách hàng

1. **Chọn danh sách khách hàng, sau đó chọn Quản lý khách hàng**

<figure><img src="../.gitbook/assets/quản lý khách hàng.png" alt=""><figcaption></figcaption></figure>

2. **Chọn các khách hàng muốn đăng ký Sequence,** sau đó **chọn Hành động, và chọn Đăng ký theo dõi kịch bản.**

<figure><img src="../.gitbook/assets/đăng ký theo dõi kịch bản.png" alt=""><figcaption></figcaption></figure>

3. **Tìm và chọn Sequence** muốn đăng ký cho khách hàng.

**Lưu ý**:

* Sequence phải được hoàn thiện trước khi đăng ký theo dõi kịch bản. Nếu không bạn phải đăng ký theo dõi kịch bản lại cho khách hàng đó.
* Sequence phải có ít nhất 1 thông điệp đã xuất bản thì khách hàng mới có thể đăng ký được.

Ngoài ra, bạn có thể thiết lập hành động Đăng ký Sequence cho khách hàng khi khách hàng kích hoạt 1 sự kiện nào đó trong Flow. Xem thêm tại [Broken link](broken-reference "mention").

### Huỷ đăng ký theo dõi kịch bản

Nếu khách hàng bạn chọn chưa được đăng ký theo dõi Sequence, thao tác vẫn thực hiện được nhưng sẽ không kích hoạt trigger Khi ai đó Huỷ đăng ký Sequence( nếu có).

1. **Chọn danh sách khách hàng, sau đó chọn Quản lý khách hàng**

<figure><img src="../.gitbook/assets/quản lý khách hàng.png" alt=""><figcaption></figcaption></figure>

2.  **Chọn các khách hàng muốn huỷ đăng ký Sequence,** sau đó **chọn Hành động,** và chọn **Huỷ đăng ký theo dõi kịch bản.**\


    <figure><img src="../.gitbook/assets/image (548).png" alt=""><figcaption></figcaption></figure>
3. **Tìm và chọn Sequence** muốn huỷ đăng ký cho khách hàng.

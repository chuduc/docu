# Chương trình khuyến mại

LadiFlow giúp bạn quản lý các chương trình khuyến mại, tạo và quản lý voucher.

### Tạo chương trình khuyến mại

1. Chọn **Cài đặt,** sau đó chọn **Chương tình khuyến mại.**

<figure><img src="../../.gitbook/assets/chương trình khuyến mại.png" alt=""><figcaption></figcaption></figure>

2. **Chọn Tạo chương trình mới.**
3. **Nhập các thông tin của chương trình khuyến mại.**\
   Nếu chọn tự động tạo mã phân phối khuyến mại, LadiFlow sẽ tạo các mã theo quy tắc bạn cài đặt mỗi khi phân phối voucher.\
   Nếu không chọn tự động tạo mã, bạn có thể tự tạo từng voucher hoặc import danh sách voucher.

#### Tạo mã voucher

1. Chọn chương trình khuyến mại muốn tạo mã voucher, sau đó chọn **Mã khuyến mại.**

<figure><img src="../../.gitbook/assets/mã khuyến mại.png" alt=""><figcaption></figcaption></figure>

2.  Chọn **Tạo mã khuyến mại mới**, sau đó chọn **tự động tạo** hoặc **tự tạo**.\


    <figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

Nếu bạn chọn tạo mã khuyến mại mới, bạn hãy nhập mã của mình và chọn **Lưu**.

Nếu bạn chọn tự động tạo mã khuyến mại, bạn hãy điền các thông tin: số lượng tạo, tiền tố (nếu có), hậu tố (nếu có). Hệ thống sẽ tự động tạo các voucher theo yêu cầu của bạn.

{% hint style="info" %}
Mã voucher do hệ thống tự tạo sẽ có thời gian hiệu lực bằng thời gian hoạt động của chương trình khuyến mại.
{% endhint %}

#### Nhập file mã voucher

Bạn có thể nhập danh sách mã voucher lên hệ thống kèm thời gian hiệu lực voucher.

1. Chọn Nhập/Xuất dữ liệu
2. Chọn Nhập dữ liệu
3. Chọn file chứa danh sách mã voucher. \
   Lưu ý, file excel yêu cầu chứa cột code

Bạn có thể tải xuống file mẫu để nhận file import bản đầy đủ.&#x20;

* code: Mã voucher
* start\_date: Ngày bắt đầu hiệu lực voucher, chấp nhận format sau\
  &#x20;dd/mm/yyyy HH:MM và yyyy/mm/dd HH:MM:ss
* expire\_date: Ngày hết hạn hiệu lực voucher, chấp nhận format sau:\
  dd/mm/yyyy HH:MM và yyyy/mm/dd HH:MM:ss
* distribute\_status: Trạng thái phân phối bao gồm: Đã phân phối và Chưa phân phối
* customer\_email: Email khách hàng được phân phối voucher
* customer\_phone: Số điện thoại khách hàng được phân phối voucher
* distribute\_date: Ngày phân phối voucher, chấp nhận format sau dd/mm/yyyy HH:MM và yyyy/mm/dd HH:MM:ss

**Lưu ý:**

* Nếu file tải lên hợp lệ, hệ thống sẽ hiển thị danh sách mã khuyến mại bạn vừa tải lên.
* Hệ thống sẽ cập nhật dữ liệu mã khuyến mại: thời gian hiệu lực, thông tin khách hàng phân phối.
* Dữ liệu khách hàng được phân phối mã khuyến mại chỉ có thể cập nhật nếu mã khuyến mại được phát ở kênh Khác và chưa được sử dụng.
*   Nếu bạn muốn hệ thống phân phối mã voucher đã nhập file, hãy tắt tính năng Tự động tạo mã khi phân phối mã khuyến mại\


    <figure><img src="../../.gitbook/assets/image (175).png" alt="" width="375"><figcaption></figcaption></figure>

#### Xem thông tin khách hàng đã phân phối voucher và trạng thái sử dụng

1. Chọn Mã voucher tại chương trình khuyến mại muốn xem
2. Chọn xem chi tiết mã voucher

<figure><img src="../../.gitbook/assets/image (177).png" alt="" width="563"><figcaption></figcaption></figure>

Với các voucher có trạng thái gửi là Đã gửi, bạn sẽ xem được thông tin khách hàng nhận voucher.&#x20;

Với các voucher có trạng thái sử dụng là Đã sử dụng, bạn sẽ xem được mã đơn hàng mà khách hàng sử dụng với voucher này.  Nếu voucher có thể sử dụng nhiều lần, danh sách mã voucher cách nhau bởi dấu phẩy như hình dưới đây.

<figure><img src="../../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

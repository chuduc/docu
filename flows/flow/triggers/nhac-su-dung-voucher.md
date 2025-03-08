# Nhắc sử dụng voucher

Bạn đã phân phối voucher cho khách hàng, khách hàng chưa hề sử dụng voucher bạn đã gửi. Bạn mong muốn nhắc khách hàng sử dụng voucher bạn đã gửi. Trigger này sẽ giúp bạn làm điều đó, các bước thiết lập như sau:

1. Tìm và chọn trigger **Nhắc sử dụng voucher**

<figure><img src="../../../.gitbook/assets/image (179).png" alt="" width="309"><figcaption></figcaption></figure>

2.  **Chọn chương trình khuyến mại mong muốn nhắc voucher**\


    <figure><img src="../../../.gitbook/assets/image (730).png" alt="" width="430"><figcaption></figcaption></figure>
3. Chọn thời gian gửi kịch bản nhắc sử dụng. Kịch bản sẽ được chạy bắt đầu từ thời gian bạn thiết lập.
4.  Chọn điều kiện thời gian voucher được gửi: sau 1 ngày, 2 ngày, 5 ngày kể từ khi phân phối voucher ....\


    <figure><img src="../../../.gitbook/assets/image (731).png" alt="" width="432"><figcaption></figcaption></figure>

{% hint style="info" %}
**Lưu ý**:

* Với 1 voucher cần nhắc sử dụng, 1 Trigger Nhắc sử dụng chỉ chạy nhiều nhất 1 lần/ ngày nếu thỏa mãn điều kiện phân phối voucher.
* Voucher có trạng thái sử dụng là Đã sử dụng thì sẽ không thể được nhắc trong trigger này.
{% endhint %}

### Gửi tin với các thông tin voucher cần nhắc sử dụng

Với Trigger nhắc sử dụng voucher, thông tin voucher cần nhắc sử dụng được lưu trong các mã code sau:

* **ldf\_voucher\_remind\_code**: mã voucher code cần nhắc
* **ldf\_voucher\_remind\_distribution\_date**: ngày phân phối voucher
* **ldf\_voucher\_remind\_expire\_date**: ngày hết hạn sử dụng voucher
* **ldf\_voucher\_remind\_start\_date**: ngày bắt đầu hiệu lực của voucher

Bạn chỉ cần nhập mã code muốn sử dụng vào nội dung tin nhắn

<figure><img src="../../../.gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

**Lưu ý:**

* Nếu tắt kích hoạt và kích hoạt lại thì hệ thống sẽ thực hiện quét các voucher thỏa mãn điều kiện và thực hiện kịch bản.
* Nếu thời gian gửi nhỏ hơn thời gian bật kích hoạt trigger, hệ thống cũng sẽ thực hiện kịch bản với tất cả các mã khuyến mại thỏa mãn điều kiện.
* Hệ thống sẽ đánh dấu voucher được sử dụng nếu có đơn hàng phát sinh. Do đó hãy đảm bảo nền tảng ecommerce, CRM đã tích hợp với LadiFlow.

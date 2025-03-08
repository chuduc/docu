# Xem danh sách khách hàng đánh giá dịch vụ tin ZNS

Nếu mẫu tin ZNS của bạn thuộc mẫu tin Đánh giá dịch vụ, LadiFlow sẽ giúp bạn xem chi tiết phản hồi của từng khách hàng khi đánh giá qua mẫu tin ZNS.

**Lưu ý:**&#x20;

* Chỉ mẫu ZNS tin thuộc loại  mẫu tin Đánh giá dịch vụ.
* Với các Flow/Sequence có mẫu tin Đánh giá dịch vụ được thiết lập trước ngày 30/01/2024, bạn cần thao tác chọn lại mẫu tin để hệ thống cập nhật dữ liệu.
* Hệ thống chỉ lưu trữ dữ liệu đánh giá từ các chiến dịch mới, các tin ZNS đã gửi sẽ không có dữ liệu đánh giá khách hàng.

Sau khi tin gửi thành công, bạn chọn xem báo cáo gửi tin ZNS đó.\


<figure><img src="../.gitbook/assets/image (641).png" alt="" width="563"><figcaption><p>Báo cáo mẫu tin ZNS đánh giá dịch vụ trong Flow</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (638).png" alt="" width="563"><figcaption><p>Báo cáo mẫu tin ZNS đánh giá dịch vụ trong Campaign</p></figcaption></figure>

Chọn **Đánh giá khách hàng** để xem chi tiết các đánh giá.

<figure><img src="../.gitbook/assets/image (640).png" alt="" width="563"><figcaption><p>Đánh giá khách hàng trong báo cáo Campaign</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (642).png" alt="" width="563"><figcaption><p>Đánh giá khách hàng trong báo cáo Flow</p></figcaption></figure>

Bạn có thể lọc theo số điểm, khoảng thời gian đánh giá hoặc sử dụng ô tìm kiếm để tìm kiếm dữ liệu mong muốn.

Các thông tin lần đánh giá gần nhất đã được lưu vào trường tùy chỉnh khách hàng sau:

**Điểm đánh giá lần cuối**:

* Tên hiển thị: Điểm đánh giá lần cuối
* Tên trường: last\_survey\_rate
* Kiểu dữ liệu: Dạng số

**Thời gian đánh giá lần cuối**

* Tên hiển thị: Thời gian đánh giá lần cuối
* Tên trường: last\_survey\_submit
* Kiểu dữ liệu: Ngày tháng

**Nội dung phản hồi**

* Tên hiển thị: Nội dung phản hồi lần cuối
* Tên trường: last\_survey\_feedback
* Kiểu dữ liệu: Danh sách

**Ghi chú phản hồi**

* Tên hiển thị: Ghi chú phản hồi lần cuối
* Tên trường: last\_survey\_note
* Kiểu dữ liệu: Đoạn văn bản

{% hint style="info" %}
**Lưu ý:** Bạn cần tạo các trường tùy chỉnh phía trên để dữ liệu đánh giá lưu thông tin vào từng khách hàng.
{% endhint %}

Bạn có thể tạo các segment với các trường tùy chỉnh này để phân loại tập khách hàng, tạo kịch bản để chăm sóc từng tập khách hàng đó.

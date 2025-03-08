# Khi đơn đặt hàng được thanh toán

Trigger sử dụng khi đơn đặt hàng được tạo hóa đơn tương ứng trên KiotViet.

1.  Chọn trigger **Khi đơn đặt hàng được thanh toán**\


    <figure><img src="../../../../.gitbook/assets/image (645).png" alt="" width="337"><figcaption></figcaption></figure>
2. Mở mục Thiết lập trigger, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").

**Lưu ý**:

* Hệ thống vẫn lưu thông tin: mã đơn hàng, doanh thu đơn hàng, các sản phẩm trong đơn hàng ... vào thông tin khách hàng đặt đơn.
* Hệ thống không lưu thông tin đơn đặt hàng vào thông tin đơn hàng của khách hàng và không ghi nhận doanh thu đối với đơn đặt hàng.
* Nếu bạn đặt các kịch bản với Trigger Khi hóa đơn được tạo, Khi hóa đơn hoàn thành thì nên thiết kế kịch bản phù hợp vì hành động tạo hóa đơn cho đơn đặt hàng sẽ thực hiện nhiều hơn 1 kịch bản.

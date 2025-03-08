# Tích hợp Haravan

Các bước tích hợp với tài khoản Haravan như sau:

1.  Tìm ứng dụng **Haravan** trên danh sách ứng dụng\


    <figure><img src="../../.gitbook/assets/image (151).png" alt="" width="563"><figcaption></figcaption></figure>
2.  Chọn **Thêm liên kết** để thêm liên kết\


    <figure><img src="../../.gitbook/assets/image (152).png" alt="" width="563"><figcaption></figcaption></figure>
3.  Điền tên tích hợp\


    <figure><img src="../../.gitbook/assets/image (153).png" alt="" width="563"><figcaption></figcaption></figure>
4.  Điền đường dẫn tài khoản Haravan vào mục **API URL**\
    \


    <figure><img src="../../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>



    <figure><img src="../../.gitbook/assets/image (154).png" alt="" width="563"><figcaption></figcaption></figure>
5. Chọn **Xác thực** để kết nối tài khoản. Khi có popup mở ra, đăng nhập vào trang Haravan của bạn.
6. Chọn đúng tài khoản với đường dẫn đã ghi ở bước 3

<figure><img src="../../.gitbook/assets/image (171).png" alt="" width="325"><figcaption></figcaption></figure>

6. Chọn **Lưu liên kết**

### Các trạng thái cơ bản đơn hàng của Haravan

Các trường dữ liệu dưới đây, nếu tài khoản của bạn chưa có, bạn có thể tự tạo với mã tương ứng. Các giá trị dưới đây có thể sẽ không đầy đủ với đơn hàng Haravan của bạn. Để chính xác, bạn thực hiện tạo đơn và kiểm tra giá trị được lưu trong các trường có mã tương ứng.

| Tên trường                 | Mã trường                     | Giá trị                                                                                                                                                                                   |
| -------------------------- | ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Last order status          | last\_order\_status           | <ul><li>pending: Đơn mới tạo</li><li>paid: Đã thanh toán</li><li>refunded: Đã hoàn trả</li><li>cancelled: Đã hủy</li></ul>                                                                |
| Last payment method        | last\_payment\_method         | <ul><li>cod: COD</li><li>bankdeposit: Chuyển khoản</li></ul>                                                                                                                              |
| Last payment status        | last\_payment\_status         | <ul><li>pending: Chưa thanh toán</li><li>paid: Đã thanh toán</li></ul>                                                                                                                    |
| Last order shipping status | last\_order\_shipping\_status | <ul><li>Chờ lấy hàng</li><li>Đang giao hàng</li><li>Đã giao</li><li>Hủy giao hàng</li><li>Chuyển hoàn</li><li>Không gặp khách</li><li>Chờ chuyển hoàn</li><li>Lấy hàng thất bại</li></ul> |

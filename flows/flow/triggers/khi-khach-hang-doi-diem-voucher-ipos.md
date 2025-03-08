# Khi khách hàng đổi điểm voucher IPOS

Khi có sự kiện khách hàng đổi điểm voucher từ IPOS, hệ thống sẽ thực hiện các kịch bản trong Flow.

### Chuẩn bị dữ liệu

Trước khi thiết lập bạn cần đảm bảo các trường tùy chỉnh sau đã có trên tài khoản của bạn:

| Mã tên trường tùy chỉnh                        | Mã trường                     | Kiểu dữ liệu |
| ---------------------------------------------- | ----------------------------- | ------------ |
| Tên chương trình khuyến mại đổi điểm cuối cùng | last\_voucher\_campaign\_name | Dòng văn bản |
| ID chương trình khuyến mại đổi điểm cuối cùng  | last\_voucher\_campaign\_id   | Dòng văn bản |
| Mã voucher đã đổi điểm                         | coupon\_code                  | Dòng văn bản |
| Điểm sau khi đổi voucher                       | point                         | Dạng số      |
| Điểm trước khi đổi voucher                     | old\_point                    | Dạng số      |
|  Hạn sử dụng voucher đổi cuối cùng             | last\_voucher\_date\_end      | Ngày tháng   |

IPOS sẽ gửi các thông tin liên quan đến chương trình khuyến mại mà khách hàng đã đổi điểm, bạn hãy tạo các trường tùy chỉnh với tên trường như trên để lấy các dữ liệu cần thiết.

### Thiết lập trigger

1.  Tìm và chọn trigger **Khi khách hàng đổi điểm voucher**\


    <figure><img src="../../../.gitbook/assets/image (621).png" alt=""><figcaption></figcaption></figure>
2. **Thêm các điều kiện thiết lập trigger nếu có**
3. **Lần lượt thêm các hành động trong Flow và xuất bản Flow**
4. **Kích hoạt trigger**

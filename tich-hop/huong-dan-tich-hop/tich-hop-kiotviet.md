# Tích hợp KiotViet

Kể từ sau thời điểm tích hợp KiotViet trên LadiFlow thành công:

* Tất cả khách hàng mới tạo đều được đồng bộ sang LadiFlow
* Tất cả đơn hàng mới tạo, cập nhật, huỷ sẽ cập nhật dữ liệu khách hàng đã có hoặc tạo mới khách hàng
* Tự động cập nhật các thông tin chỉ số liên quan đến đơn hàng của bạn và của từng khách hàng

### Các bước tích hợp Kiotviet

1. Tìm và chọn ứng dụng **KiotViet** trên danh sách ứng dụng tích hợp.

<figure><img src="../../.gitbook/assets/image (409).png" alt=""><figcaption></figcaption></figure>

2. Chọn **Thêm liên kết.**
3. Mở thêm 1 cửa sổ trình duyệt, truy cập vào kiotviet và đăng nhập với shop của bạn.
4. Tại trang **KiotViet**, Chọn **Setting**, chọn **Thiết lập cửa hàng**, sau đó chọn **Thiết lập kết nối API.**
5. Điền thông tin Tên kết nối trùng với tên cửa hàng bạn đã đăng ký. Sau đó chọn **Lưu**.

<figure><img src="../../.gitbook/assets/image (441).png" alt=""><figcaption></figcaption></figure>

6. Sau đó copy lần lượt **Tên kết nối, Client ID, Mã bảo mật** trên **KiotViet** và paste vào **Form trên LadiFlow.**
7. Điền **Tên tích hợp**.
8. Sau đó chọn **Lưu kết nối**.

{% hint style="info" %}
Hiện tại hệ thống không giới hạn số tích hợp KiotViet.
{% endhint %}

### Lưu dữ liệu từ Kiotviet vào trường tùy chỉnh

**Sau khi tích hợp KiotViet thành công, khi có Đơn đặt hàng mới, Hóa đơn mới thì dữ liệu khách hàng sẽ tự động về dữ liệu tài khoản LadiFlow của bạn.  Các dữ liệu đơn hàng, hóa đơn và khách hàng được tự động lưu vào các trường tùy chỉnh tương ứng.**&#x20;

**Ngoài ra với 1 số thông tin đặc thù của từng nền tảng, bạn cần phải tạo các trường tùy chỉnh tương ứng:**

**Tổng nợ của khách hàng**

* Tên hiển thị: Tổng nợ của khách hàng
* Tên trường: debt
* Kiểu dữ liệu: Dạng số

**Tổng số tiền thanh toán trong hóa đơn**

* Tên hiển thị: Tổng số tiền thanh toán trong hóa đơn cuối
* Tên trường: last\_total\_payment\_amount
* Kiểu dữ liệu: Dạng số

**ID cửa hàng**

* Tên hiển thị: ID cửa hàng Kiotviet
* Tên trường: last\_retailer\_id
* Kiểu dữ liệu: Dòng văn bản

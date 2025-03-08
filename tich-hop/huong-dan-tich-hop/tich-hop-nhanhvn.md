# Tích hợp Nhanhvn

Để tích hợp Nhanhvn trên LadiFlow, tài khoản Nhanh của bạn cần cấp quyền truy cập API. Bạn thực hiện như sau trên Nhanhvn:

1. Vào Cài đặt, sau đó chọn Cài đặt chung

<figure><img src="../../.gitbook/assets/image (674).png" alt=""><figcaption></figcaption></figure>

2. Bật Cài đặt Open API.

<figure><img src="../../.gitbook/assets/image (675).png" alt=""><figcaption></figcaption></figure>

### **Thao tác thêm mới tích hợp Nhanhvn trên LadiFlow**

1.  Tìm ứng dụng Nhanhvn trong thư viện tích hợp\


    <figure><img src="../../.gitbook/assets/image (155).png" alt="" width="563"><figcaption></figcaption></figure>
2. Chọn **Thêm liên kết**

<figure><img src="../../.gitbook/assets/image (156).png" alt="" width="563"><figcaption></figcaption></figure>

3.  **Điền Tên tích hợp**\


    <figure><img src="../../.gitbook/assets/image (157).png" alt="" width="563"><figcaption></figcaption></figure>
4.  Chọn **Kết nối với Nhanh và đăng nhập tài khoản Nhanh**\


    <figure><img src="../../.gitbook/assets/image (158).png" alt="" width="563"><figcaption></figcaption></figure>
5. Điền tên tích hợp và **chọn Lưu liên kết**

### Các trường tùy chỉnh dữ liệu khách hàng

Các mã trường tùy chỉnh dưới đây, nếu bạn cần dữ liệu nào hãy tạo trường tùy chỉnh tương ứng vào tài khoản. Hệ thống sẽ tự động lưu dữ liệu vào các trường dữ liệu này.

| Mã trường                      | Loại dữ liệu | Mô tả                                                                                                       |
| ------------------------------ | ------------ | ----------------------------------------------------------------------------------------------------------- |
| nhanhvn\_type                  | Dạng số      | Loại khách hàng (1 = Khách lẻ, 2 = Khách buôn, 3 = Đại lý)                                                  |
| nhanhvn\_code                  | Dòng văn bản | Mã khách hàng                                                                                               |
| nhanhvn\_level                 | Dòng văn bản | Tên cấp độ( level) của khách hàng                                                                           |
| nhanhvn\_group                 | Dòng văn bản | Nhóm khách hàng                                                                                             |
| nhanhvn\_total\_money          | Dạng số      | Tổng số tiền khách mua hàng                                                                                 |
| nhanhvn\_point                 | Dạng số      | Điểm tích lũy hiện tại của khách hàng                                                                       |
| first\_order\_created\_date    | Ngày tháng   | Ngày đầu tiên mua hàng                                                                                      |
| last\_order\_created\_date     | Ngày tháng   | Ngày cuối cùng mua hàng. Trường này được cập nhật giá trị khi có đơn hàng, hóa đơn bán sỉ, bán lẻ.          |
| last\_order\_mode              | Dòng văn bản | <p>Loại hóa đơn cuối cùng:<br>2: bán lẻ<br>6: bán sỉ</p>                                                    |
| nhanhvn\_last\_sale\_name      | Dòng văn bản | Tên nhân biên bán hàng của hóa đơn bán sỉ, bán lẻ cuối cùng                                                 |
| last\_order\_created\_by\_name | Dòng văn bản | Tên nhân viên thu ngân hóa đơn bán sỉ, bán lẻ cuối cùng                                                     |
| last\_order\_payment\_amount   | Dạng số      | Số tiền đã thanh toán tại đơn hàng cuối                                                                     |
| last\_order\_date              | Ngày tháng   | Ngày cuối cùng phát sinh đơn hàng, hóa đơn. Giá trị này không đổi nếu nhiều đơn phát sinh trong cùng 1 ngày |
| nhanhvn\_first\_depot\_name    | Dòng văn bản | Tên chi nhánh mua hàng đầu tiên( Đối với khách hàng mới sau khi tích hợp)                                   |
| nhanhvn\_first\_depot\_id      | Dòng văn bản | ID chi nhánh mua hàng đầu tiên( Đối với khách hàng mới sau khi tích hợp)                                    |
| nhanhvn\_last\_depot\_name     | Dòng văn bản | Tên chi nhánh mua hàng cuối cùng                                                                            |
| nhanhvn\_last\_depot\_id       | Dòng văn bản | ID chi nhánh mua hàng cuối cùng                                                                             |

# Tích hợp IPOS



Trước tiên, bạn cần yêu cầu IPOS thêm LadiPage thành đối tác trên tài khoản IPOS của bạn. Các bước làm như sau:

1. Gửi email tới support@ipos.vn với nội dung như sau:

Thân gửi quý đối tác,&#x20;

<\<Tên thương hiệu>> xác nhận cho phép LadiFlow nhận các sự kiện liên quan đến dữ liệu của <\<Tên thương hiệu>> trên IPOS thông qua webhook: [https://api.service.ladiflow.com/1.0/webhook/ipos](https://api.service.ladiflow.com/1.0/webhook/ipos)

Quý đối tác vui lòng hỗ trợ <\<tên thương hiệu>> triển khai setup.

Trân trọng cảm ơn!

2. Chờ bên IPOS thiết lập xong và đội ngũ LadiFlow xác nhận IPOS đã thiết lập thành công.
3. Sau khi IPOS đã cho phép LadiFlow nhận dữ liệu từ thương hiệu của bạn. Bạn tìm ứng dụng **IPOS** trên danh sách thư viện tích hợp.\


<figure><img src="../../.gitbook/assets/image (148).png" alt="" width="563"><figcaption></figcaption></figure>

4. Chọn **Thêm liên kết.**\


<figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

5. Nhập ID thương hiệu và nhập tên tích hợp.\
   Trong trường hợp không biết ID thương hiệu, đội ngũ LadiFlow sẽ gửi lại ID thương hiệu cho bạn.

<figure><img src="../../.gitbook/assets/image (141).png" alt="" width="563"><figcaption></figcaption></figure>

Bật Tự động đồng bộ CTKM từ CRM IPOS thì các Chương trình khuyến mại phát hành trên kênh đối tác LadiPage sẽ tự động được tạo trên tài khoản LadiFlow của bạn.

6. Chọn **Lưu liên kết** để lưu lại.

**Hiện tại hệ thống không giới hạn số tích hợp IPOS.**

**Lưu ý:** Mỗi thương hiệu chỉ được tích hợp với 1 tài khoản LadiFlow.

### Lưu dữ liệu từ IPOS vào trường tùy chỉnh <a href="#luu-du-lieu-tu-kiotviet-vao-truong-tuy-chinh" id="luu-du-lieu-tu-kiotviet-vao-truong-tuy-chinh"></a>

Các mã trường tùy chỉnh dưới đây, nếu bạn cần dữ liệu nào hãy tạo trường tùy chỉnh tương ứng vào tài khoản. Hệ thống sẽ tự động lưu dữ liệu vào các trường dữ liệu này.

<table><thead><tr><th width="201">Mã trường</th><th width="166">Loại dữ liệu</th><th>Mô tả</th></tr></thead><tbody><tr><td>last_pos_name</td><td>Dạng văn bản</td><td> Cửa hàng mua lần cuối</td></tr><tr><td>last_point</td><td>Dạng số</td><td>Số điểm tích lũy của đơn hàng cuối cùng</td></tr></tbody></table>


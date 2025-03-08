# Khách hàng checkin sự kiện LadiPage Ecommerce

Khi khách hàng check sự kiện được bán vé qua LadiPage Ecommerce bạn có thể gửi tin chăm sóc khách hàng ngay khi khách hàng checkin. Các bước thiết lập như sau:

1. Chọn **Trigger Check-in sự kiện LadiPage Ecommerce**

<figure><img src="../../../.gitbook/assets/image (669).png" alt=""><figcaption></figcaption></figure>

2. **Chọn tài khoản cấu hình LadiPage Ecommerce**

<figure><img src="../../../.gitbook/assets/image (670).png" alt="" width="469"><figcaption></figcaption></figure>

3. **Chọn sự kiện và loại vé tương ứng**. Nếu bạn không chọn mặc định tất cả các sự kiện sẽ đều chạy kịch bản này

<figure><img src="../../../.gitbook/assets/image (671).png" alt="" width="476"><figcaption></figcaption></figure>

4. Thêm lần lượt các hành động vào Flow, xuất bản Flow và kích hoạt trigger

### Thông tin các trường thông tin của sự kiện LadiPage Ecommerce

Để lấy, lưu trữ thông tin sự kiện check in của từng khách hàng, bạn tạo các trường tùy chỉnh sau vào tài khoản của bạn. \
Lưu ý: Nếu không cần dữ liệu nào, bạn không cần phải tạo trường tùy chỉnh đó

| Tên hiển thị      | Tên trường                    | Kiểu dữ liệu |
| ----------------- | ----------------------------- | ------------ |
| ID mã ghế         | lds\_event\_ticket\_seat\_id  | Dòng văn bản |
| ID sự kiện        | lds\_event\_id                | Dòng văn bản |
| ID loại vé        | lds\_event\_ticket\_id        | Dòng văn bản |
| Thời gian checkin | lds\_event\_checked\_in\_time | Ngày tháng   |
| Tên sự kiện       | lds\_event\_name              | Dòng văn bản |
| Tên loại vé       | lds\_event\_ticket\_name      | Dòng văn bản |
| Mã vé             | lds\_event\_ticket\_code      | Dòng văn bản |

{% hint style="info" %}
Nếu bạn thường xuyên diễn ra các sự kiện, hãy đặt hành động Gắn tag tham gia sự kiện với từng khách hàng checkin. Sau khi sự kiện kết thúc, bạn có thể Segment Check-in sự kiện và tập khách hàng không tham dự sự kiện dựa vào các khách hàng được gắn tag tham gia sự kiện.
{% endhint %}

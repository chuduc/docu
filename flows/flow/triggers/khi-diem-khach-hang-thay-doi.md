---
description: Sự kiện điểm Lead Score của khách hàng thay đổi
---

# Khi điểm khách hàng thay đổi

Trigger hoạt động khi điểm (Score) của khách hàng có sự thay đổi.

Trigger được kích hoạt bằng cách

* Cập nhật điểm khách hàng thủ công tại Chỉnh sửa thông tin khách hàng
* Điểm được thay đổi khi thực hiện hành động **Điều chỉnh Lead Scoring** trong Flow, Sequence, Campaign khác

1. Chọn **+Thêm trigger** và **chọn trigger Khi điểm khách hàng thay đổi.**

<figure><img src="https://lh5.googleusercontent.com/yXfp0dlIAxum0xlcDIrP9tduRLCXLpq3Ww9ZZSTqjNJpDzdutceHCkKWJD2tGpl7SNQqGuxeQAFHbFfabdUqUlI5TyhLzOdXN9Z_8VNBbCF-uAAuXxPAwac7dvoX_FkijblYCrkfrGLlAf-hm3LXeS0" alt=""><figcaption></figcaption></figure>

2. Điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
3. **Chọn toán tử so sánh và điền số điểm so sánh.**\
   Bạn có thể chọn các toán tử so sánh: lớn hơn, lớn hơn hoặc bằng, nhỏ hơn…. để làm điều kiện chạy trigger. Khi đó nếu giá trị điểm của khách hàng sau khi thay đổi thoả mãn điều kiện, flow sẽ thực hiện với khách hàng đó.

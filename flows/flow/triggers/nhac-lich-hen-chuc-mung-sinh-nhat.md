---
description: Sự kiện tạo lịch hẹn, chúc mừng sinh nhật.. cho khách hàng
---

# Nhắc lịch hẹn, chúc mừng sinh nhật

Trigger được dùng khi đặt lịch nhắc, lịch hẹn dựa theo các trường thông tin thời gian của khách hàng như: thư chúc mừng sinh nhật, thông báo đơn hàng...

1. Chọn **+Thêm Trigger**, **tìm và chọn Nhắc lịch hẹn.**

<figure><img src="../../../.gitbook/assets/image (779).png" alt=""><figcaption></figcaption></figure>

1. Điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
2. **Điền các thông tin thiết lập thời gian và điều kiện gửi lịch hẹn.**

<figure><img src="../../../.gitbook/assets/image (334).png" alt=""><figcaption></figcaption></figure>

Nếu muốn đặt lịch hẹn theo thông tin của khách hàng: thư chúc mừng sinh nhật, thông báo đơn hàng.... hãy chọn trường thông tin điều kiện và chọn tuần suất hàng ngày.

{% hint style="info" %}
**Tần suất:** là tần suất hệ thống quét các bản ghi thỏa mãn điều kiện, không phải tần suất gửi kịch bản.&#x20;

**Ví dụ**: bạn đặt tần suất hàng tuần và vào thứ 2, thì mỗi thứ 2 hàng tuần hệ thống quét các khách hàng thỏa mãn điều kiện nhắc lịch và thực hiện kịch bản theo thời gian đã thiết lập.
{% endhint %}

**Lưu ý:**

* Hệ thống sẽ thực hiện quét danh sách khách hàng thỏa mãn điều kiện và thực hiện kịch bản với khách hàng đó.&#x20;
* Nếu khách hàng đã được thực hiện Nhắc lịch, bạn thay đổi dữ liệu khách hàng thì khách hàng đó sẽ KHÔNG được thực hiện kịch bản.
* Nếu bạn tắt trigger, kích hoạt lại trigger thì hệ thống cũng sẽ không thực hiện kịch bản với các khách hàng mà ngày hôm đó đã được thực hiện kịch bản.
* Khi kích hoạt lại trigger sau khi đã chỉnh sửa, lịch hẹn cũ sẽ bị xoá, hệ thống gửi lịch hẹn theo dữ liệu trigger mới.

---
description: Sự kiện thay đổi thông tin tuỳ chỉnh của khách hàng
---

# Khi một Trường thông tin tùy chỉnh thay đổi

Trigger hoạt động khi trường thông tin tuỳ chỉnh của khách hàng thay đổi theo điều kiện thiết lập.

Trường thông tin tuỳ chỉnh là các trường thông tin mà bạn tự tạo để lưu trữ thêm dữ liệu khách hàng ngoài các thông tin mặc định trên LadiFlow. Để tạo trường tuỳ chỉnh bạn xem thêm tại [truong-tuy-chinh.md](../../../cai-dat/cai-dat-chung/truong-tuy-chinh.md "mention").

Trigger được kích hoạt khi:

* Cập nhật thủ công dữ liệu trường thông tin tuỳ chỉnh trên thông tin khách hàng
* Tự động cập nhật khi hành động **Thêm trường tùy chỉnh** được thực hiện trên Flow, Sequence, Campaign khác

1. **Chọn +Thêm Trigger**, tìm và chọn Trigger **Trường tuỳ chỉnh thay đổi.**

<figure><img src="../../../.gitbook/assets/image (481).png" alt=""><figcaption></figcaption></figure>

2. Chọn điều kiện kích hoạt trigger nếu muốn giới hạn tập khách hàng của flow, xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
3. **Chọn phương thức điều kiện**: Tất cả các điều kiện hoặc Điều kiện bất kỳ.

{% hint style="info" %}
Tất cả các điều kiện tương đương với biểu thức logic Và (AND).

&#x20;Điều kiện bất kỳ tương đương với biểu thức logic Hoặc (OR).
{% endhint %}

4. **Chọn Thêm trường tuỳ chỉnh,** sau đó **điền thông tin điều kiện so sánh.**

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-21 at 11.27.50.png" alt=""><figcaption></figcaption></figure>

5. Thêm trường tuỳ chỉnh nếu muốn thêm điều kiện trường thông tin.
6. Xoá trường tuỳ chỉnh nếu muốn.



<figure><img src="../../../.gitbook/assets/xoá điều kiện.png" alt=""><figcaption><p>Xoá trường tuỳ chỉnh</p></figcaption></figure>

**Lưu ý**:&#x20;

* Nếu điều kiện trả ra tập rỗng, bạn vẫn có thể kích hoạt và xuất bản flow nhưng sẽ không có khách hàng nào áp dụng flow.
* Trường tùy chỉnh thay đổi chỉ được chạy nếu nó thực sự thay đổi. Nếu 2 lần cập nhật cùng 1 giá trị thì trigger cũng sẽ không thực hiện.

---
description: Khi các trường thông tin mặc định của khách hàng được cập nhật
---

# Khi một Trường thông tin mặc định thay đổi

Trigger hoạt động khi có trường thông tin mặc định của khách hàng đã cài đặt thay đổi giá trị. Trường thông tin mặc định là các trường mặc định của LadiFlow, không phải các trường tuỳ chỉnh do bạn tạo.

Trigger hoạt động khi:

* Bạn tự cập nhật thủ công thông tin khách hàng.
* Tự động cập nhật thông tin khách hàng khi có dữ liệu đơn hàng.
* Tự động tạo mới khách hàng khi khách hàng từ Facebook, Zalo hoặc kích hoạt trigger từ Flow khác.

<mark style="color:red;">**Lưu ý**</mark>:

* Cẩn trọng khi cài đặt Trigger với trường Email, họ và tên, số điện thoại vì bạn sẽ có thể không kiểm soát được số lượng Flow thực hiện với khách hàng

1. **Chọn Thêm mới Trigger**, tìm và chọn **Trigger Trường mặc định thay đổi.**

<figure><img src="https://lh5.googleusercontent.com/le3zjPKcipOhXUY-15yiJOlqwcMHhLHdebaQ3xECD3_8H6w_dXJwsUG43Qc7ovKIx3Tzcd2e4OpKM2TPz73VwyS9EDwoFwo7QTCu6fBSFEm5gPMPTkszBcZFs_iVK89RJCfO36nIVwOee6mRzDl_cxI" alt=""><figcaption></figcaption></figure>

2. Chọn điều kiện kích hoạt trigger nếu muốn giới hạn tập khách hàng của flow, xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
3. **Chọn phương thức điều kiện:** Tất cả các điều kiện hoặc Điều kiện bất kỳ.

{% hint style="info" %}
Tất cả các điều kiện tương đương với biểu thức logic Và (AND).

&#x20;Điều kiện bất kỳ tương đương với biểu thức logic Hoặc (OR).
{% endhint %}

4. **Chọn Thêm trường tuỳ chỉnh**, sau đó chọn trường thông tin đặt điều kiện và điều kiện áp dụng.

Dưới đây là danh sách các trường mặc định và điều kiện so sánh:

<figure><img src="../../../.gitbook/assets/trường mặc định.png" alt=""><figcaption></figcaption></figure>

5. Xoá trường tuỳ chỉnh nếu muốn.

<figure><img src="../../../.gitbook/assets/xoá điều kiện.png" alt=""><figcaption><p>Xoá điều kiện</p></figcaption></figure>

**Lưu ý:**&#x20;

* Nếu điều kiện trả ra tập rỗng, bạn vẫn có thể kích hoạt và xuất bản Flow nhưng sẽ không có khách hàng nào áp dụng Flow.
* Trường tùy chỉnh thay đổi chỉ được chạy nếu nó thực sự thay đổi. Nếu 2 lần cập nhật cùng 1 giá trị thì trigger cũng sẽ không thực hiện.

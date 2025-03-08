---
description: Khi đơn hàng chuyển sang trạng thái đã huỷ.
---

# Khi một đơn hàng bị hủy

Trigger hoạt động khi có 1 đơn hàng bị huỷ trên LadiSales, Shopify, Haravan, Sapo, Woocomerce, Nhanh.vn,... Tuỳ theo từng nền tảng, bạn chọn trigger Đơn hàng bị huỷ tương ứng. Bạn phải tích hợp tài khoản với các nền tảng trên để trigger hoạt động.

{% hint style="info" %}
Bạn phải tích hợp tài khoản với các nền tảng trên để trigger hoạt động.
{% endhint %}

**Lưu ý lựa chọn hành động phù hợp với Trigger:**

* SMS, AI Call, Zalo ZNS nếu có thông tin số điện thoại tại đơn hàng hoặc đã có dữ liệu số điện thoại của khách hàng trên LadiFlow
* Gửi Email nếu có thông tin địa chỉ email( đã xác thực) của khách hàng trên đơn hàng hoặc trên LadiFlow
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....
* Các hành động khác: gửi tin Zalo Quan tâm, Messenger sẽ không thể thực hiện được nếu khách hàng đó chưa từng tương tác với Page Facebook hoặc tài khoản Zalo OA của bạn.

1. **Chọn +Thêm trigger**, tìm và **chọn trigger Đơn hàng bị huỷ** như hình dưới đây.

<figure><img src="../../../.gitbook/assets/đơn hàng bị huỷ.png" alt=""><figcaption><p>Trigger Đơn hàng bị huỷ trên LadiSales</p></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Mở mục Thiết lập Trigger**, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").

**Lưu ý**: &#x20;

* Dựa theo email trong đơn hàng, hệ thống thực hiện trigger với khách hàng đó.
* Khi đơn hàng bị huỷ, LadiFlow tạo mới một khách hàng trên danh sách khách hàng của bạn nếu email khách hàng trong đơn chưa có trên LadiFlow, ngược lại hệ thống tự động cập nhật dữ liệu theo thông tin đơn hàng.&#x20;
* Trigger Khi một đơn hàng huỷ không thể thực hiện hành động Gửi tin Zalo quan tâm và gửi tin Messager nếu chưa có tài khoản Zalo, Facebook của khách hàng đó.

---
description: khi ai đó bỏ giỏ hàng trên LadiSales.
---

# Khi ai đó bỏ giỏ hàng

Trigger hoạt động khi sản phẩm được thêm vào giỏ hàng thành công nhưng không tạo đơn hàng trên LadiSales. Tuỳ theo từng nền tảng, bạn chọn Trigger bỏ giỏ hàng tương ứng. Bạn phải tích hợp tài khoản với các nền tảng trên để Trigger hoạt động.

{% hint style="info" %}
Bạn phải tích hợp tài khoản với các nền tảng trên để trigger hoạt động.
{% endhint %}

**Lưu ý lựa chọn hành động phù hợp với Trigger:**

* SMS, AI Call, Zalo ZNS nếu đã có dữ liệu số điện thoại của khách hàng trên LadiFlow.
* Gửi Email nếu đã có dữ liệu email (đã xác thực) của khách hàng trên LadiFlow.
* Các hành động của LadiFlow: gắn tag, bỏ tag, đăng ký Sequence...
* Các hành động khác: gửi tin Zalo, Messenger sẽ không thể thực hiện được nếu khách hàng đó chưa từng tương tác với Page Facebook hoặc tài khoản Zalo OA của bạn.

1.  **Chọn +Thêm Trigger,** tìm và **chọn trigger Sản phẩm được thêm vào giỏ hàng** theo nền tảng mong muốn.\


    <figure><img src="../../../.gitbook/assets/image (524).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Mở mục Thiết lập Trigger**, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").

**Lưu ý**:&#x20;

* Khi có ai đó thêm sản phẩm vào giỏ hàng, LadiFlow tạo mới một khách hàng trên danh sách khách hàng của bạn nếu email khách hàng chưa có trên LadiFlow, ngược lại hệ thống tự động cập nhật dữ liệu theo thông tin mà LadiSales, Haravan cung cấp.
* Dựa theo email của khách hàng trên LadiSales và Haravan, hệ thống thực hiện Trigger với khách hàng đó trên LadiFlow.
* Các Trigger Khi sản phẩm được thêm vào giỏ hàng không thể thực hiện hành động Gửi tin Zalo quan tâm và gửi tin Messager nếu chưa có tài khoản Zalo, Facebook của khách hàng đó.

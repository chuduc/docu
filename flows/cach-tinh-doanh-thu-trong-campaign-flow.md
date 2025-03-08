# Cách tính doanh thu trong Campaign, Flow

LadiFlow đã có thể tính doanh thu từ Campaign, Flow thông qua kênh gửi Email. Bài viết này sẽ giúp bạn hiểu rõ hơn cách ghi nhận doanh thu trên LadiFlow.

Doanh thu trên Flow, Campaign qua kênh gửi Email đều có chung cách thức ghi nhận như sau:

* Email gửi có chứa link đặt hàng.
* Khách hàng đặt đơn hàng qua Link gửi trong Email.

1. **Email gửi có chứa link đặt hàng.**

Link đặt hàng có thể là Link dẫn sang sản phẩm, trang thanh toán hoặc Trang chủ cửa hàng của bạn. Miễn sao từ Link này khách hàng có thể phát sinh đơn hàng.

2. **Khách hàng đặt đơn hàng qua Link gửi trong Email**

Khách hàng phải Click, truy cập từ Link trong Email bạn gửi, sau đó phát sinh đơn hàng thì hệ thống mới ghi nhận doanh thu cho Email gửi tin. Nếu khách hàng truy cập trực tiếp vào cửa hàng, Link sản phẩm và đặt đơn không qua Email thì hệ thống không ghi nhận doanh thu.

{% hint style="info" %}
Bạn lưu ý, bạn cần tích hợp với nền tảng E-commerce( Woocomerce, Haravan, LadiPage Ecommerce ...) tương ứng trên LadiFlow để hệ thống nhận được dữ liệu đơn hàng khi có đơn hàng mới.
{% endhint %}

### Nếu đơn hàng cập nhật thay đổi thì doanh thu trên LadiFlow sẽ như thế nào?

Hệ thống ghi nhận doanh thu Campaign, Flow tại thời điểm đặt đơn. Nếu sau đó đơn hàng cập nhật, hủy, hoàn thì doanh thu Campaign, Flow sẽ không cập nhật lại.

# Nhanhvn- Hóa đơn bán lẻ, bán sỉ mới

Trigger thực hiện khi có hóa đơn bán lẻ, bán si mới được tạo trên Nhanhvn. Dữ liệu hóa đơn bán lẻ, bán sỉ sẽ được lưu như một đơn hàng trên LadiFlow. Các bước thiết lập trigger như sau:

1.  Tìm và chọn trigger **Hóa đơn bán lẻ, bán sỉ mới**\


    <figure><img src="../../../.gitbook/assets/image (676).png" alt="" width="228"><figcaption></figcaption></figure>
2. Mở mục Thiết lập trigger, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").

Để phân biệt hóa đơn bán lẻ, bán sỉ bạn đặt điều kiện như hình sau:

*   Chỉ thực hiện kịch bản nếu là hóa đơn bán lẻ\


    <figure><img src="../../../.gitbook/assets/image (677).png" alt="" width="317"><figcaption></figcaption></figure>
*   Chỉ thực hiện kịch bản nếu là hóa đơn bán sỉ\


    <figure><img src="../../../.gitbook/assets/image (678).png" alt="" width="323"><figcaption></figcaption></figure>

{% hint style="info" %}
Nếu bạn không có trường last\_order\_mode, bạn có thể tạo mới trường tùy chỉnh với mã last\_order\_mode. Ngoài ra, để sử dụng các dữ liệu khác liên quan đến hóa đơn từ Nhanhvn, bạn xem thêm tại [#cac-truong-tuy-chinh-du-lieu-khach-hang](../../../tich-hop/huong-dan-tich-hop/tich-hop-nhanhvn.md#cac-truong-tuy-chinh-du-lieu-khach-hang "mention")
{% endhint %}

# Phân phối voucher

Khi bạn muốn phân phối voucher cho khách hàng của bạn. Trước tiên bạn cần phải có chương trình khuyến mại để có danh sách voucher trước. Nếu chưa có, xem hướng dẫn tạo tại [chuong-trinh-khuyen-mai.md](../../../cai-dat/cai-dat-chung/chuong-trinh-khuyen-mai.md "mention")

{% hint style="info" %}
Hành động này chỉ thực hiện được khi bạn đã có tập khách hàng trên LadiFlow.
{% endhint %}

### Thêm hành động phân phối voucher

Đây là hành động hệ thống lấy voucher từ chương trình khuyến mại hoặc tạo voucher mới.

1. **Chọn +Thêm hành động**, tìm và **chọn hành động Phân phối voucher.**
2. **Chọn chương trình khuyến mại.**&#x20;

**Lưu ý**:&#x20;

* Chương trình khuyến mại được chọn phải được kích hoạt tại thời điểm thực hiện hành động.
* Chỉ các chương trình khuyến mại đang trong thời gian hiệu lực, hệ thống mới có thể gửi thông tin voucher cho khách hàng của bạn.
* Nếu bạn tắt Tự động tạo mã voucher tại chương trình khuyến mại, bạn phải đảm bảo đã có sẵn danh sách mã voucher tại chương trình khuyến mại đó.

### Gửi thông tin voucher cho khách hàng

Tại nội dung các hành động gửi tin nhắn, email bạn gắn thông tin voucher cho khách hàng bằng cách thêm biến tuỳ chỉnh \{{voucher\_code\}}.&#x20;

**Lưu ý**:&#x20;

* nếu bạn chưa chọn hành động phân phối voucher trước khi gửi cho khách hàng, khách hàng có thể không nhận được mã hoặc nhận được mã voucher gần nhất mà bạn đã gửi.
* Trong cùng 1 flow, mỗi lần bạn phân phối voucher, hệ thống sẽ chọn hoặc tạo ra voucher chưa gửi để gửi cho khách hàng( tùy theo thiết lập của chương trình khuyến mại).&#x20;

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

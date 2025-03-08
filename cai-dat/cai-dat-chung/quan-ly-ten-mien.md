# Quản lý tên miền



Nếu bạn đã có tên miền (Business Email), bạn hãy sử dụng tên miền để gửi email. Đầu tiên, bạn cần thêm và xác thực tên miền.

1. Chọn **Cài đặt**, sau đó chọn **Quản lý tên miền.**
2. Chọn **Thêm tên miền**.
3. **Nhập tên miền** của bạn.
4. Chọn **Thêm tên miền.** Sau khi thêm tên miền thành công, hệ thống hiển thị danh sách các bản ghi DNS cần thêm như sau:

<figure><img src="../../.gitbook/assets/image (23).png" alt="" width="563"><figcaption></figcaption></figure>

6. Truy cập vào kênh quản lý tên miền của bạn, **tạo lần lượt các bản ghi DNS với các thông tin hệ thống hiển thị**.&#x20;
7. Chờ khi Trạng thái Tracking SSL đã được bật, bấm **Xác thực.**

<figure><img src="../../.gitbook/assets/image (16).png" alt="" width="563"><figcaption></figcaption></figure>

Xem thêm hướng dẫn tạo bản ghi trên trang quản lý tên miền tại [cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien](../../cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien/ "mention")

{% hint style="info" %}
**Lưu ý:**&#x20;

* Bản ghi cần khoảng thời gian vài phút tới vài tiếng để áp dụng, do đó hãy chờ nhiều nhất 1 ngày.
* 1 tên miền chưa xác thực có thể được thêm tại nhiều tài khoản, nhưng tên miền xác thực chỉ có thể xác thực tại 1 tài khoản. Khi đó, các tài khoản khác có tên miền này sẽ không thể xác thực và sử dụng được.
{% endhint %}

{% hint style="info" %}
Trạng thái xác thực tên miền trên LadiFlow là trạng thái xác thực DKIM. Để kiểm tra các phương thức xác thực SPF, DMARC vui lòng xem hướng dẫn sau [#chu-dong-kiem-tra-xac-thuc-danh-tinh-dkim-spf-dmarc](../../meo-su-dung-ladiflow/cac-luu-y-khi-gui-email-bang-domain-cua-ban.md#chu-dong-kiem-tra-xac-thuc-danh-tinh-dkim-spf-dmarc "mention")
{% endhint %}

### Xác thực DKIM

DKIM là 1 trong số các phương pháp để xác thực tên miền, khi được xác thực danh tính người gửi của bạn sẽ được tăng lên. Do đó, tỷ lệ vào inbox tăng, tỷ lệ vào spam giảm.

{% hint style="info" %}
LadiFlow tự động thêm bản ghi vào tên miền để xác thực DKIM, bạn cần tạo lần lượt các bản ghi trên kênh quản lý tên miền của bạn.
{% endhint %}

Xem các lưu ý khi xác thực DKIM tại [#luu-y-khi-xac-thuc-dkim](../../meo-su-dung-ladiflow/cac-luu-y-khi-gui-email-bang-domain-cua-ban.md#luu-y-khi-xac-thuc-dkim "mention").

### **Xác thực SPF**

1. Bạn cần chọn nền tảng gửi và nhận mail để lấy bản ghi SPF.&#x20;
2. Sau đó tạo bản ghi DNS theo dữ liệu của LadiFlow.

<figure><img src="../../.gitbook/assets/image (18).png" alt="" width="563"><figcaption><p>Bản ghi SPF</p></figcaption></figure>

Bạn chỉ có thể tạo một bản ghi SPF cho tên miền của mình. Nếu bạn có bản ghi SPF hiện có, bạn sẽ cần phải sửa đổi bản ghi hiện có của mình thay vì tạo bản ghi SPF mới.

Các lưu ý khi tạo bản ghi SPF tại đây [#luu-y-khi-xac-thuc-spf](../../meo-su-dung-ladiflow/cac-luu-y-khi-gui-email-bang-domain-cua-ban.md#luu-y-khi-xac-thuc-spf "mention").

### Xác thực DMARC

Bạn cần tạo bản ghi DMARC giống như LadiFlow yêu cầu.

<figure><img src="../../.gitbook/assets/image (19).png" alt="" width="563"><figcaption><p>Bản ghi DMARC</p></figcaption></figure>

{% hint style="info" %}
Để kiểm tra xác thực và các lưu ý khi tạo bản ghi, vui lòng xem thêm tại [cac-luu-y-khi-gui-email-bang-domain-cua-ban.md](../../meo-su-dung-ladiflow/cac-luu-y-khi-gui-email-bang-domain-cua-ban.md "mention")
{% endhint %}

{% hint style="info" %}
Khi tên miền đã được **xác thực**, bạn có thể sử dụng bằng cách tích hợp thêm Email tên miền đó, xem thêm tại đây [tich-hop-email.md](../../tich-hop/huong-dan-tich-hop/tich-hop-email.md "mention").
{% endhint %}

### Bản ghi TRACKING

Việc nhất quán thông tin người gửi, tên miền, và các liên kết trong email sẽ quyết định tỷ lệ email của bạn sẽ vào SPAM.&#x20;

_**Cụ thể**: **Nếu bạn dùng tên miền ladipage.vn để gửi thì các liên kết trong email cũng phải sử dụng link với ladipage.vn dưới dạng thư mục con hoặc tên miền phụ.**_

Do vậy, LadiFlow cung cấp bản ghi Tracking và hỗ trợ bật SSL để tăng độ xác thực danh tính người gửi và tăng độ tin cậy cho email của bạn.

* **Bản ghi Tracking** được sử dụng để theo dõi được lượt mở và lượt click link trong các chiến dịch email của bạn.

Bạn cần tạo bản ghi Tracking theo dữ liệu LadiFlow cung cấp để chúng tôi có thể tracking được chiến dịch email của bạn.&#x20;

Xem thêm hướng dẫn tạo bản ghi trên trang quản lý tên miền tại [cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien](../../cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien/ "mention")

<figure><img src="../../.gitbook/assets/image (20).png" alt="" width="563"><figcaption><p>Bản ghi Tracking</p></figcaption></figure>

* **Trạng thái SSL:** Là trạng thái SSL của trackingdns.email.tenmiencuaban. Gồm 2 trạng thái: Chưa bật và Đã bật.

SSL sẽ được bật tự động sau khi bạn trỏ bản ghi Tracking.&#x20;

Thời gian để hệ thống bật SSL thành công là từ 0 đến 2 giờ sau khi xác thực tên miền.

{% hint style="info" %}
Trường hợp SSL không được bật sau 2 giờ, vui lòng liên hệ chúng tôi để được hỗ trợ.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (24).png" alt="" width="563"><figcaption><p>Trạng thái Chưa bật</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (22).png" alt="" width="563"><figcaption><p>Trạng thái Đã bật</p></figcaption></figure>

{% hint style="danger" %}
Trường hợp SSL chưa được bật: Khi truy cập đường dẫn trong email của bạn, trình duyệt web sẽ hiển thị cảnh báo **"Trang web không an toàn".**&#x20;

Điều này ảnh hưởng tới độ tin cậy và bảo mật dữ liệu của đường dẫn, đồng nghĩa với việc email của bạn sẽ có nguy cơ bị đánh dấu là spam.
{% endhint %}

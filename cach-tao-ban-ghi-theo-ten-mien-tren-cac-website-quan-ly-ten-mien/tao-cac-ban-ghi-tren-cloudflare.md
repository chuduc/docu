# Tạo các bản ghi trên cloudflare

Trong trường hợp bạn chưa có tài khoản cloudflare, bạn thực hiện các bước sau:

**Bước 1: Đăng ký tài khoản tại** [**https://www.cloudflare.com**](https://www.cloudflare.com/)**.**&#x20;

**Bước 2: Thêm Website vào CloudFlare.**

Đầu tiên bạn bấm Add a Site để thêm tên miền của bạn vào hệ thống CloudFlare. Bạn nhập tên miền chính không có www.\


<figure><img src="../.gitbook/assets/image (628).png" alt="" width="563"><figcaption></figcaption></figure>

**Bước 3: Lựa chọn Plan.**

CloudFlare có khá nhiều plan với các chức năng cao cấp, tuy nhiên bạn có thể Free Plan.

<figure><img src="../.gitbook/assets/image (629).png" alt=""><figcaption></figcaption></figure>

* Sau khi chọn Free rồi nhấn Confirm Plan, bạn tiếp tục các bước của Cloudflare.

**Bước 4. Xác thực các cấu hình đã có của tên miền.**

* Nếu tên miền đang hoạt động, toàn bộ các bản ghi bạn đã tạo trong quản trị tên miền sẽ được CloudFlare quét và hiển thị lại
* Có thể xuất hiện trường hợp không có bản ghi nào cả, nếu tên miền vừa được đăng ký xong.

**Bước 5: Trỏ Name servers về CloudFlare.**

CloudFlare cung cấp 2 bản ghi Name servers, bạn sao chép 02 Namesever này thay thế cho 02 Nameserver của bên cung cấp tên miền. Trong trường hợp bạn không biết thao tác thay đổi nameserver trong quản trị tên miền, xin vui lòng liên hệ với bên cung cấp tên miền, nhờ hỗ trợ thay đổi Nameserver về 2 bản ghi Name server của Cloudflare.

<figure><img src="../.gitbook/assets/image (630).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Lưu ý:**&#x20;

Khi đã trỏ Nameserver về CloudFlare, cấu hình các bản ghi trong quản trị tên miền sẽ không còn hiệu lực. Tất cả các ghi sẽ được tạo/cập nhật trong tài khoản CloudFlare.
{% endhint %}

### Tạo bản ghi

Bạn truy cập vào mục DNS để tạo các bản ghi tên miền.

<figure><img src="../.gitbook/assets/image (631).png" alt=""><figcaption></figcaption></figure>

**\*Lưu ý:** tắt biểu tượng đám mây như ảnh hướng dẫn cho bản gh&#x69;**.**

au khi tạo đầy đủ các bản ghi, quay trở lại LadiFlow, chọn **Xác thực** tên miền bạn vừa thêm bản ghi. Nếu trạng thái Đã xác thực, bạn có thể sử dụng tên miền này để gửi Email. Nếu Xác thực lỗi, hãy kiểm tra lại danh sách bản ghi trên LadiFlow và trên cloudflare.


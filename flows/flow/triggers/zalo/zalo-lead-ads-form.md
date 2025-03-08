# Zalo lead ads form

Khi có ai đó hoàn thành form của Zalo lead ads, trigger sẽ hoạt động.&#x20;

{% hint style="info" %}
Lựa chọn trigger này nếu tập khách hàng của bạn thường xuyên tương tác với bạn/doanh nghiệp qua Zalo
{% endhint %}

**Điều kiện hoạt động trigger**:

* Tài khoản Zalo tích hợp đã có Lead Ads
* Các thông tin mapping dữ liệu đúng

1.  **Chọn +Thêm trigger,** tìm và chọn trigger **Zalo Lead Ads Form.**\


    <figure><img src="../../../../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Chọn tài khoản Zalo cấu hình**. Đây là tài khoản sẽ chạy Lead ads form, nếu bạn chưa có hãy tích hợp thêm( xem thêm tại [tich-hop-zalo.md](../../../../tich-hop/huong-dan-tich-hop/tich-hop-zalo.md "mention"))

**Lưu ý**: Tài khoản zalo của bạn phải là tài khoản Zalo OA.

<figure><img src="../../../../.gitbook/assets/image (714).png" alt="" width="425"><figcaption></figcaption></figure>

3. Mở mục Thiết lập trigger, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Điền ID của form. Để lấy ID form bạn thực hiện như sau:**
   1.  Chọn chi tiết chiến dịch, sau đó chọn **Tải dữ liệu Form**\


       <figure><img src="https://lh7-us.googleusercontent.com/tdbtQXtTACDVG4bMqVf8Q3QdiJQholFJUhjVaRC-cUbtIhWLD8nFB8QpHX7kkpkZMtUkof0NNnlMbaXe85wjli5p8P3enaRI2PJYmwnkMrU8hftuaxG7jrLtPpCxcJk4sIG22ZKWhvCGMDPTiDXf_A" alt="" width="563"><figcaption></figcaption></figure>


   2. Sao chép ID form bằng cách Copy dữ liệu trong ô Tìm kiếm hoặc lấy trên đường dẫn (giá trị sau từ search=, trước \&oaId)

<figure><img src="https://lh7-us.googleusercontent.com/W7V5yVRohI4QGg6BQC6tLSyBZXaKAxPZjR-L0ogjOI5H_GghcylmtMxFqyq2ooIXM2_aOZE36FgOVDfFtxqQ7_RIhtmlKo3G8LYLepfD6HixSoKZEcOGFQjRYsBuzYQc4Vl1yv2NWV-xicKV5o0tuw" alt="" width="563"><figcaption></figcaption></figure>

4. **Điền các trường thông tin mapping dữ liệu.**&#x20;

<figure><img src="../../../../.gitbook/assets/image (388).png" alt=""><figcaption></figcaption></figure>

Phía bên phải bạn chọn các trường thuộc tính của khách hàng trên Ladiflow. Đây là các trường thông tin bạn muốn lưu dữ liệu tương ứng với dữ liệu khách hàng nhập tại form bên trái.

Phía bên trái, tương ứng với mỗi thuộc tính trên LadiFlow, bạn điền tên tiêu đề của từng câu hỏi trên Form ads.

<figure><img src="../../../../.gitbook/assets/lead ads zalo.png" alt=""><figcaption></figcaption></figure>

Được kết quả như sau.

<figure><img src="../../../../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>

**Lưu ý:** Bạn cần điền đúng chính tả thông tin thuộc tính Zalo để dữ liệu được cập nhật đúng.

6. **Kiếm tra tài khoản Zalo** để đảm bảo tài khoản của bạn vẫn hoạt động.

**Lưu ý:**&#x20;

* Với dữ liệu khách hàng nhập trên Form, hệ thống tự động cập nhật thông tin khách hàng trên LadiFlow dựa theo thông tin mapping trong trigger.
* Với khách hàng đã có, hệ thống tự động cập nhật dữ liệu mới dựa trên dữ liệu trên Form khách hàng nhập.

**Gợi ý các hành động phù hợp:**

* Các hành động trên LadiFlow: gắn tag, đăng ký sequence...
* Gửi Zalo quan tâm.
* Gửi thông báo Telegram, Slack, Email.

# Zalo Chat Keywords

Trigger hoạt động khi có ai đó nhắn tin cho tài khoản Zalo OA( Zalo Account Official) mà bạn đã tích hợp. Bạn có thể tuỳ chỉnh điều kiện tin nhắn kích hoạt trigger: chứa/loại trừ các từ khoá cụ thể, tất cả tin nhắn.

{% hint style="info" %}
Lựa chọn trigger này nếu tập khách hàng của bạn thường xuyên tương tác với bạn/doanh nghiệp qua Zalo
{% endhint %}

**Lưu ý**:

* LadiFlow tự động thêm thông tin khách hàng trong tập khách hàng của bạn ngay khi có ai đó nhắn tin tới tài khoản Zalo OA mà bạn đã tích hợp
* Để có tài khoản Zalo OA, bạn phải đăng ký với Zalo.

1.  **Chọn Thêm trigger,** tìm và chọn **Trigger Zalo Chat Keywords.**\


    <figure><img src="../../../../.gitbook/assets/image (543).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Chọn tài khoản zalo cấu hình trigger**. Nếu bạn chưa có tài khoản nào, hãy tích hợp thêm( xem thêm tại [tich-hop-zalo.md](../../../../tich-hop/huong-dan-tich-hop/tich-hop-zalo.md "mention"))

**Lưu ý**: tài khoản zalo của bạn phải là tài khoản Zalo OA.\


<figure><img src="../../../../.gitbook/assets/image (712).png" alt="" width="436"><figcaption></figcaption></figure>

3. Mở mục Thiết lập trigger, điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Chọn điều kiện nội dung tin nhắn**: tin nhắn chứa từ khoá bất kỳ, tin nhắn chứa từ khoá cụ thể:

* **Nếu bạn chọn tin nhắn chưa từ khoá bất kỳ**, trigger sẽ hoạt động với tất cả tin nhắn khách hàng gửi cho bạn.
* N**ếu bạn chọn tin nhắn chứa từ khoá cụ thể**, **bạn hãy nhập từ khoá mong muốn, sau đó nhấn enter để thêm từ khoá như hình dưới đây:**

<figure><img src="../../../../.gitbook/assets/nhap tu khoa 2.gif" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (567).png" alt=""><figcaption></figcaption></figure>

5. **Điền danh sách từ khoá loại trừ nếu có.**&#x20;
6.  Bật/Tắt điều kiện kích hoạt trigger khi nội dung tin nhắn chưa email, số điện thoại. \


    <figure><img src="../../../../.gitbook/assets/image (713).png" alt="" width="422"><figcaption></figcaption></figure>
7. Chọn lưu địa chỉ email, số điện thoại trong tin nhắn nếu muốn cập nhật thông tin khách hàng theo email và số điện thoại khách hàng theo dữ liệu khách hàng gửi trong tin nhắn.
8. **Kiểm tra tài khoản zalo** của bạn để chắc chắn trigger hoạt động.

**Gợi ý các hành động phù hợp:**

* Các hành động trên LadiFlow: gắn tag, đăng ký sequence...
* Gửi Zalo quan tâm
* Gửi thông báo Telegram, Slack, Email.

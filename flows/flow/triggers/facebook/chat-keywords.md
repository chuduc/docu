---
description: Sự kiện khi có khách hàng nhắn tin với Page Facebook của bạn.
---

# Chat Keywords

Trigger hoạt động khi có tin nhắn mới tới page của bạn trên Facebook. Bạn có thể tuỳ chỉnh từ khoá trong tin nhắn của khách hàng để kích hoạt trigger.

1.  Chọn +**Thêm trigger** và **tìm trigger Facebook Chat Keywords.**\


    <figure><img src="../../../../.gitbook/assets/image (539).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2.  **Chọn tài khoản cấu hình Facebook**. Nếu bạn chưa có tài khoản nào, hãy tích hợp thêm.\


    <figure><img src="../../../../.gitbook/assets/image (701).png" alt="" width="433"><figcaption></figcaption></figure>
3. Chọn mục Thiết lập trigger, thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Nếu bạn muốn gửi tin với các khách hàng Lần đầu nhắn tin với Page, bắt đầu cuộc trò chuyện với Page sau 1 khoảng thời gian** thì bạn **Chọn Chỉ chạy trigger với khách hàng thoả mãn điều kiện nhắn tin lần cuối**

<figure><img src="../../../../.gitbook/assets/image (667).png" alt="" width="473"><figcaption></figcaption></figure>



3. **Chọn khoảng thời gian khách nhắn tin lần cuối tương ứng:** \
   **Ví dụ**: nếu bạn cài đặt 8 giờ, cứ sau ít nhất 8 giờ kể từ lần cuối khách hàng phản hồi tin nhắn với Page của bạn, hệ thống sẽ gửi các kịch bản tin nhắn tương ứng.\
   Nếu khách hàng lần đầu nhắn tin với page cũng sẽ được thực hiện kịch bản.
4. **Chọn điều kiện kích hoạt trigger**: tin nhắn chứa từ khoá cụ thể, tin nhắn chứa từ khoá bất kỳ.
5.  **Nhâp từ khoá chứa và loại trừ (nếu có). Để nhập từ khoá, bạn hãy nhập từ khoá mong muốn, sau đó nhấn enter để thêm từ khoá như hình dưới đây:**\


    <figure><img src="../../../../.gitbook/assets/nhập từ khóa fb.gif" alt="" width="308"><figcaption></figcaption></figure>



    <figure><img src="../../../../.gitbook/assets/image (564).png" alt=""><figcaption></figcaption></figure>
6.  Bật/Tắt điều kiện hoạt động của trigger khi tin nhắn có chứa email hoặc số điện thoại.\
    \


    <figure><img src="../../../../.gitbook/assets/image (704).png" alt="" width="426"><figcaption></figcaption></figure>
7.  Chọn lưu lại địa chỉ email, số điện thoại trong tin nhắn nếu bạn muốn tự động cập nhật địa chỉ email, số điện thoại của khách hàng theo email và số điện thoại mà khách hàng gửi.\


    <figure><img src="../../../../.gitbook/assets/image (705).png" alt="" width="427"><figcaption></figcaption></figure>
8. **Chọn mục kiểm tra, kiểm tra tài khoản Facebook của bạn** để đảm bảo Trigger sẽ hoạt động.

{% hint style="info" %}
**Lưu ý**:&#x20;

* Khi có 1 người gửi tin nhắn tới page, hệ thống tự động tạo 1 khách hàng trên LadiFlow nếu đó là khách hàng mới.
* Nếu bạn thiết lập lưu địa chỉ email, số điện thoại trong tin nhắn và email khách hàng nhập trùng với dữ liệu đã có trên tập khách hàng của bạn thì hệ thống sẽ không cập nhật email vào thông tin khách hàng Facebook.
{% endhint %}

**Gợi ý các hành động phù hợp với Trigger:**

* **Gửi tin nhắn Messenger**
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....

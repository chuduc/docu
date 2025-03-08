# Chỉnh sửa dữ liệu trang tính Google sheet

### Trigger này đã ngừng cho phép tạo mới vào 17/04/2024

Trigger hoạt động khi một trang tính của bạn được thay đổi dữ liệu.&#x20;

{% hint style="info" %}
Sử dụng trigger khi bạn đã có file sheet thông tin khách hàng.
{% endhint %}

**Lưu ý:**

* **Trang tính của bạn bắt buộc phải có cột thông tin Email hoặc số điện thoại** của khách hàng.
* Trang tính của bạn được chỉnh sửa thủ công mới kích hoạt trigger này.
* Hệ thống sẽ dựa theo thông tin email, số điện thoại tại hàng có ô tính được chỉnh sửa dữ liệu để thực hiện các hành động với khách hàng đó.
* Hệ thống tự động thêm thông tin của khách hàng dựa theo dữ liệu tại hàng có ô tính chứa dữ liệu thay đổi.

**Gợi ý các hành động phù hợp với các trigger:**

* Các hành động trên LadiFlow: gắn tag, đăng ký sequence...
* Gửi Email nếu đã có thông tin địa chỉ email (đã xác thực) tại hàng có ô tính thay đổi.
* Gửi SMS, Zalo ZNS, AI call nếu đã có thông tin số điện thoại tại hàng có ô tính thay đổi.
* Messenger nếu khách hàng của bạn đã/đang tương tác với bạn qua Messenger.
* Gửi thông báo Telegram, Slack, Email.

1. **Chọn +Thêm Trigger,** tìm và **chọn trigger Hàng tính mới được thêm hoặc chỉnh sửa.**
2. **Chọn tài khoản Google Sheet tích hợp**. Đây là tài khoản chứa trang tính của bạn, nếu bạn chưa có tài khoản nào hãy tích hợp thêm.
3. Chọn mục Thiết lập Trigger, thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
4.  **Chọn trang tính mà bạn muốn thực hiện Trigger.**

    Bạn có thể tạo mới trang tính ngay trên LadiFlow với tài khoản Google Sheet đã tích hợp\
    Bạn cũng có thể điền ID bảng tính thay vì điền tên. ID của bảng tính lấy dựa theo đường dẫn của bảng tính đó.

<figure><img src="../../../.gitbook/assets/id sheet.png" alt=""><figcaption><p>ID trang tính trên google sheet</p></figcaption></figure>

5. **Chọn Sheet lấy dữ liệu.** Đây là Trang tính mọi sự thay đổi dữ liệu trên ô tính, hệ thống sẽ thực hiện cập nhật dữ liệu khách hàng tại hàng có ô tính thay đổi dữ liệu.
6. **Chọn Cột tính thay đổi dữ liệu.**&#x20;

* Nếu bạn chọn cột tính, chỉ khi dữ liệu thay đổi tại cột đã chọn thì Trigger mới được chạy.
* Nếu bạn không chọn cột tính, bất kì sự thay đổi tại bất kỳ ô tính nào Trigger cũng chạy.&#x20;

7. **Điền thông tin mapping dữ liệu.** Bên phải là trường dữ liệu của khách hàng trên LadiFlow, bên trái là các cột lấy dữ liệu tương ứng. \
   Hệ thống tự động lấy hàng 1 trên sheet để làm dữ liệu mapping.

{% hint style="info" %}
Dữ liệu mapping phải có dữ liệu số điện thoại hoặc email thì mới thực hiện hành động trong Flow.
{% endhint %}

8. **Sao chép mã nhúng, nhúng vào trang tính của bạn.**
9. **Kiểm tra tài khoản đảm bảo tài khoản google sheet của bạn vẫn đang hoạt động.**

**Lưu ý**:&#x20;

* **Tài khoản cấu hình phải có quyền sửa trang tính mà bạn chọn.**
* Khi Trigger được kích hoạt, bất cứ sự thay đổi nào trên dữ liệu ô tính, hệ thống cũng cập nhật thông tin khách hàng tại hàng đó. Do đó trên sheet bạn chọn phải có ít nhất 1 cột dữ liệu Email hoặc số điện thoại khách hàng.
* **Chỉ cài đặt 1 trang tính 1 trigger duy nhất để đảm bảo Flow thực hiện đúng.**
* **Sau khi thay đổi lại trang tính đã chọn, hãy cập nhật thông tin mã nhúng trên trang tính.**

### Thêm mã nhúng vào trang tính

1. Copy mã nhúng trên trigger.

<figure><img src="../../../.gitbook/assets/copy mã nhúng.png" alt=""><figcaption></figcaption></figure>

2. **Mở trang tính của bạn** .
3. **Chọn Tiện ích mở rộng, sau đó chọn Apps Script.**

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-25 at 14.13.03.png" alt=""><figcaption></figcaption></figure>

4. **Xác nhận uỷ quyền truy cập** bằng cách chọn Xem lại quyền.

<figure><img src="../../../.gitbook/assets/uỷ quyền.png" alt=""><figcaption></figcaption></figure>

4. **Dán mã nhúng vào Apps Script** và **bấm tổ hợp Ctrl+ s để lưu dự án.**

<figure><img src="../../../.gitbook/assets/add script.png" alt=""><figcaption></figcaption></figure>

4. **Chọn hàm setupWebhook** và **chọn chạy dự án.**

<figure><img src="../../../.gitbook/assets/run app script.png" alt=""><figcaption></figcaption></figure>

5.  **Chọn tài khoản thực thi**. Tài khoản này phải có quyền chỉnh sửa trang tính trên.

    <figure><img src="https://lh4.googleusercontent.com/kK6BDToKlgtaxERNQ8orJxRgYd363AjfJi37NOlwojUULHxd0nQZEfG_Sm584fLCo05YNfNR-fMR-VWtm0JzfCwQ9KnvnK2q5Z2HJurliRHBFFVacqKgRdnEOR-21KmP-CsmxcLdsJTbayEfuymK7g" alt=""><figcaption></figcaption></figure>
6.  **Chọn Allow để xác nhận quyền truy cập.**

    <figure><img src="https://lh5.googleusercontent.com/0Um0FylJbNnpwgN54PPx-19B-3kJ4bQ36VpZaNjDMsVHGpmgJOkaGG8Pwd9wiAqsXaxB8OPGITDJcn27ntl1MKHoqBwpx0KBf2RyatxLdZBALBzIXj5_ITRH-0YhXkWUvCx5dAe4MZryfXEDuXfvvQ" alt=""><figcaption></figcaption></figure>
7. **Chờ đợi hệ thống chạy cho đến khi hoàn tất**. Nếu nhật ký thực thi báo lỗi, hãy chạy lại.

<figure><img src="../../../.gitbook/assets/run success.png" alt=""><figcaption></figcaption></figure>

8. **Mở Kích hoạt** kiểm tra đã tạo được hàm onEdit. Như vậy bạn đã cài mã nhúng cho Sheet của bạn thành công.

<figure><img src="https://lh6.googleusercontent.com/bvY8Q2KmGVLkND1VyAim6-xFtnGywwMU6RBjRdhOjKu1Ts0J8iOUm70fqAL-mr9hDor3l-fvnUF1KCqlhg3UgzBd-um4QP3Hnry208zRE3c2UICDLXH1QcV8AU2FQhH4_uxEJAd6oECu3Vq0accarg" alt=""><figcaption></figcaption></figure>

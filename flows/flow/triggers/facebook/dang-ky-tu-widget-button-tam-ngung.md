---
description: Sự kiện Khách hàng nhấn vào button nhắn tin với Page trên website của bạn
---

# Đăng ký từ Widget Button (Tạm ngừng)

{% hint style="danger" %}
Facebook đã thông báo ngừng hỗ trợ tính năng Plugin Send to Messenger kể từ ngày 30/09/2024. Do đó, tính năng tạo mới trigger Đăng ký từ Widget Button Facebook trên LadiFlow sẽ tạm thời không khả dụng.&#x20;

Để biết thêm thông tin chi tiết về thay đổi này, vui lòng tham khảo tại: [https://developers.facebook.com/docs/messenger-platform/discovery/send-to-messenger-plugin](https://developers.facebook.com/docs/messenger-platform/discovery/send-to-messenger-plugin)
{% endhint %}

Nếu bạn muốn gắn nút "Send to Messenger" trên Website của bạn, để khách hàng có thể trực tiếp truy cập tới Page trên Facebook, bạn hãy sử dụng Trigger Subscribe từ Widget Button.&#x20;

<figure><img src="../../../../.gitbook/assets/image (587).png" alt=""><figcaption></figcaption></figure>

Trigger hoạt động khi có bất kỳ người nào click vào Button trên **website đã gắn SDK button của LadiFlow** . Khi click vào nút, khách hàng sẽ được điều hướng sang trang nhắn tin với Page trên Messager hoặc đường dẫn đã cài đặt trong Flow.

**Lưu ý**:&#x20;

* Trigger chỉ có thể hoạt động khi website của bạn có mã nhúng của Trigger LadiFlow.
* Khi có 1 người nhấn vào Button trên website, hệ thống tự động tạo 1 khách hàng trên LadiFlow nếu đó là khách hàng mới.
* Chỉ thực hiện hành động với những ai click và Button đã cài đặt trên website của bạn.

1. Chọn **+ Thêm Trigger** và chọn **Subcribe từ Widget Button.**

<figure><img src="https://lh4.googleusercontent.com/r3vpU8M_wrpifuywLf3G_EwX0y1adKXPKdLhLqJLCnqrl_tVatNd-o_Pi8JafBZEGNiWLWMPW3GxzmdkEvh3eyFyQVFtlYd7w_YX2EV7GO-a9e7IYHSXw_fxklsdOjE6Ri-c6nGGt5d8rQFVhyQzYwE" alt="" width="375"><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

2. **Chọn tài khoản cấu hình**, đây là page trên Facebook bạn muốn khách hàng điều hướng tới. Nếu không có tài khoản nào, hãy tích hơp thêm.

<figure><img src="https://lh4.googleusercontent.com/lskcb-8a1aU2friOVBZNO1Nx-Ph10mehi149Evjmk63F-NGDKnUCtnshOAOgPf3CJn9yvsEm87PeFHV4OpSLkuS8hBSKXQuF-sYmlkfRKXLe1LsdRakzdixgkF4UqprxN71ENqXrODy410dHDfsJJ5s" alt=""><figcaption></figcaption></figure>

3. **Mở mục Thiết lập trigger,** điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Chỉnh sửa giao diện của nút** bằng cách chọn kích thước, màu sắc, nội dung trước và sau khi khách hàng click.

<figure><img src="../../../../.gitbook/assets/image (692).png" alt="" width="419"><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (693).png" alt="" width="416"><figcaption></figcaption></figure>

Bạn có thể xem trước hình ảnh của nút tương ứng với từng phong cách nút bạn chọn

<figure><img src="../../../../.gitbook/assets/image (694).png" alt="" width="426"><figcaption></figcaption></figure>

3. **Điền URL điều hướng** nếu bạn muốn điều hướng sang đường dẫn khác không phải là nhắn tin với page.
4. **Kiểm tra tài khoản** để đảm bảo rằng tài khoản Facebook của bạn vẫn đang hoạt động.

**Gợi ý các hành động phù hợp với Trigger:**

* **Gửi tin nhắn Messenger**
* Hành động trên LadiFlow: gắn tag, bỏ tag, đăng ký Sequence....

### Gắn SDK và button vào Landing Page/Website của bạn trên LandiPage

**Button đăng ký mặc định ở đầu trang**

1. Mở chi tiết landing page của bạn trên LadiPage
2. Chọn Mã JavaScript/CSS

<figure><img src="../../../../.gitbook/assets/image (570).png" alt="" width="248"><figcaption></figcaption></figure>

3. Sao chép SDK trong chi tiết Trigger&#x20;

<figure><img src="../../../../.gitbook/assets/image (571).png" alt=""><figcaption></figcaption></figure>

4. Dán vào mục Trước thẻ \</head> trên LadiPage

<figure><img src="../../../../.gitbook/assets/image (572).png" alt="" width="375"><figcaption></figcaption></figure>

5. Sao chép Mã nhúng ng chi tiết Trigger trên LadiFlow

<figure><img src="../../../../.gitbook/assets/image (573).png" alt=""><figcaption></figcaption></figure>

6. Thêm phần tử Mã HTML vào trang landing page của bạn

<figure><img src="../../../../.gitbook/assets/image (575).png" alt=""><figcaption></figcaption></figure>

7. Chọn **Sửa HTML**&#x20;

<figure><img src="../../../../.gitbook/assets/image (695).png" alt=""><figcaption></figcaption></figure>

8. Dán mã nhúng button đã sao chép vào biểu mẫu Chỉnh sửa HTML

&#x20;

<figure><img src="../../../../.gitbook/assets/image (696).png" alt="" width="563"><figcaption></figcaption></figure>

9. Xuất bản landing page để xem và kiểm tra sdk và button vừa gắn.

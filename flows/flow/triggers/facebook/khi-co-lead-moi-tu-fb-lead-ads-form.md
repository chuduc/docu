---
description: Sự kiện khi có khách hàng xác nhận biểu mẫu Facebook Lead ads Form.
---

# Khi có Lead mới từ FB Lead Ads Form

### I. Hướng dẫn tạo Lead Ads Form trên Facebook

Nếu bạn đã tạo Lead Ads Form sẵn thì hãy kiểm tra lại lần lượt các bước theo hướng dẫn ở đây để đảm bảo đã thiết lập chính xác.

1. Truy cập vào đường dẫn [https://business.facebook.com/](https://business.facebook.com/)
2. Chọn **All tools**, sau đó chọn **Instant Forms**

<figure><img src="../../../../.gitbook/assets/image (183).png" alt="" width="540"><figcaption></figcaption></figure>

3. Chọn Create Form để tạo Form

<figure><img src="../../../../.gitbook/assets/image (184).png" alt="" width="563"><figcaption></figcaption></figure>

4. Chọn New Form nếu bạn muốn tạo Form mới. Nếu muốn chỉnh sửa Form đã có, chọn Duplicate existing form.

<figure><img src="../../../../.gitbook/assets/image (185).png" alt="" width="563"><figcaption></figcaption></figure>

5. Lần lượt điền các thông tin tổng quan về Form

<figure><img src="../../../../.gitbook/assets/image (186).png" alt="" width="563"><figcaption></figcaption></figure>

7. Chọn mục Questions để điền các câu hỏi trong Form. Có rất nhiều loại câu hỏi khác nhau trên Form: Câu hỏi chọn đáp án, câu hỏi điền đáp án... Tùy theo yêu cầu của bạn hãy thiết lập nội dung form thích hợp.

<figure><img src="../../../../.gitbook/assets/image (187).png" alt="" width="563"><figcaption><p>Câu hỏi điền đáp án</p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (188).png" alt="" width="563"><figcaption><p>Câu hỏi chọn đáp án</p></figcaption></figure>

8. Sau khi đã thiết lập tất cả các câu hỏi cho Forms, chọn Settings sau đó chuyển trạng thái Sharing sang Open

<figure><img src="../../../../.gitbook/assets/image (189).png" alt="" width="563"><figcaption></figcaption></figure>

9. Chọn Field names để thiết lập dữ liệu.  Để dữ liệu được lưu vào đúng trên LadiFlow, bạn hãy diền mã tên các trường tùy chỉnh tương ứng với từng câu hỏi.&#x20;

<figure><img src="../../../../.gitbook/assets/image (190).png" alt=""><figcaption></figcaption></figure>

Để biết các mã bạn có thể xem tại tính năng Cá nhân hóa

<figure><img src="../../../../.gitbook/assets/image (191).png" alt="" width="324"><figcaption></figcaption></figure>

Mã code sẽ hiển thị tương ứng trong cặp \{{\}} khi bạn chọn trường dữ liệu tương ứng.

<figure><img src="../../../../.gitbook/assets/image (192).png" alt="" width="326"><figcaption></figcaption></figure>

Nếu bạn muốn lưu thông tin vào 1 trường dữ liệu chưa tồn tại trên tài khoản, bạn có thể Tạo mới trường tùy chỉnh, xem thêm tại [truong-tuy-chinh.md](../../../../cai-dat/cai-dat-chung/truong-tuy-chinh.md "mention")

10. Sau khi đã thiết lập đầy đủ các mã tên trường dữ liệu trên LadiFlow và các thông tin khác, bạn chọn **Create Form** để tạo Form

{% hint style="info" %}
Form đã tạo thì không thể chỉnh sửa. Do đó bạn hãy nhân bản Form để chỉnh sửa lại hoặc tạo mới Form khác.
{% endhint %}

### II. Hướng dẫn thiết lập Trigger FB Lead Ads Form trên LadiFlow

Khi có ai đó gửi thông tin điền từ form trên Facebook lead ads, Trigger sẽ hoạt động.

{% hint style="info" %}
Hãy thiết lập Facebook Lead Ads trên Facebook trước khi thiết lập Trigger. Nếu bạn chưa tạo Facebook Lead Ads Form, xem hướng dẫn TẠI ĐÂY.
{% endhint %}

1.  **Chọn + Thêm Trigger**, tìm và chọn trigger **Lead từ FB Lead Ads Form**.\


    <figure><img src="../../../../.gitbook/assets/image (542).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Bạn có thể sử dụng công cụ tìm kiếm để tìm Trigger nhanh hơn.
{% endhint %}

1.  **Chọn tài khoản Facebook cấu hình**, đây là tài khoản Facebook có chứa Lead Ads.\


    <figure><img src="../../../../.gitbook/assets/image (710).png" alt="" width="427"><figcaption></figcaption></figure>
2. C**họn mục Thiết lập trigger,** thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](../them-dieu-kien-kich-hoat-trigger.md "mention").
3. **Chọn Lead Form** kích hoạt trigger từ danh sách lead form của bạn.

{% hint style="info" %}
Hãy tạo Lead form trên tài khoản Facebook của bạn trước khi thiết lập Trigger.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (711).png" alt="" width="287"><figcaption></figcaption></figure>

4. **Chọn Kiểm tra** để kiểm tra tài khoản Facebook của bạn vẫn đang hoạt động.
5. Bật **Kích hoạt Trigger**.

{% hint style="info" %}
**Lưu ý:**

* Hệ thống tự động cập nhật thông tin khách hàng theo các trường tùy chỉnh thiết lập trong Form.&#x20;
* Với dữ liệu khách hàng nhập trên Form, hệ thống tự động cập nhật thông tin khách hàng trên LadiFlow.
* Với khách hàng đã có, hệ thống tự động cập nhật dữ liệu mới dựa trên dữ liệu trên Form khách hàng nhập.
* Chỉ khi trigger được bật, dữ liệu khách hàng nhập Form mới được ghi nhận trên LadiFlow
{% endhint %}

#### III. Kiểm tra Lead Ads Form đã tạo

1. Truy cập vào màn hình Danh sách Forms trên [https://business.facebook.com/](https://business.facebook.com/)
2. Chọn Form muốn kiểm tra và chọn Test Form

<figure><img src="../../../../.gitbook/assets/image (193).png" alt="" width="375"><figcaption></figcaption></figure>

3. Khi bạn Submit Form test, dữ liệu sẽ tự động được gửi về LadiFlow. Bạn hãy kiểm tra trong danh sách khách hàng và thông tin khách hàng bạn vừa submit. Nếu dữ liệu của khách hàng thiếu dữ liệu trên Form, hãy kiểm tra lại các mã code dữ liệu đã gắn trên Form tại Bước 9 ở trên.

{% hint style="info" %}
Với mỗi tài khoản Facebook, khi bạn đã submit form test rồi và muốn thực hiện kiểm tra lại bạn cần thực hiện Xóa khách hàng tiềm nằng:

* Truy cập vào [https://developers.facebook.com/tools/lead-ads-testing](https://developers.facebook.com/tools/lead-ads-testing)
* Chọn Page và Form
*   Chọn Delete Lead

    <figure><img src="../../../../.gitbook/assets/image (181).png" alt="" width="563"><figcaption></figcaption></figure>
{% endhint %}

Sau khi kiểm tra các dữ liệu đã về LadiFlow đủ và chính xác, bạn có thể bắt đầu tạo quảng cáo FB lead ads form để thực hiện thu lead.

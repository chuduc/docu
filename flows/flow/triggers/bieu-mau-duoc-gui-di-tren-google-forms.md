---
description: Sự kiện khi khách hàng gửi biểu mẫu Google Forms.
---

# Biểu mẫu được gửi đi trên Google Forms

Trigger hoạt động khi có ai đó xác nhận Gửi biểu mẫu Google Form nếu các thông tin đều hợp lệ.

**Lưu ý:**

* Biểu mẫu bạn tạo bắt buộc phải yêu cầu nhập email hoặc số điện thoại&#x20;

**Gợi ý các hành động phù hợp với trigger:**

* Gửi Email: nếu trong biểu mẫu yêu cầu nhập email bắt buộc
* SMS, Zalo ZNS, AI Call nếu trong biểu mẫu yêu cầu nhập số điện thoại bắt buộc
* Các hành động khác của LadiFlow: gắn tag, đăng ký sequence,...

1.  **Chọn +Thêm Trigger**, tìm và **chọn trigger Biểu mẫu được gửi đi trên Google Forms.**\


    <figure><img src="../../../.gitbook/assets/image (532).png" alt=""><figcaption></figcaption></figure>
2. **Chọn tài khoản Google Forms.**
3. Chọn mục Thiết lập trigger, thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
4. **Chọn biểu mẫu thiết lập Trigger**. Nếu bạn chưa có biểu mẫu nào hãy tạo mới biểu mẫu trên ứng dụng Google Forms.
5. **Chọn dữ liệu mapping**. Bên phải là danh sách các trường thông tin của khách hàng, bên trái là câu hỏi tương ứng với câu trả lời trong biểu mẫu.

{% hint style="info" %}
Hệ thống tự động cập nhật dữ liệu khách hàng dựa trên email hoặc tạo mới khách hàng với các dữ liệu mà bạn mapping.

Nếu bạn mapping sai kiểu dữ liệu hệ thống yêu cầu, trigger sẽ không hoạt động được.
{% endhint %}

6. Chọn **Thêm trường dữ liệu** để thêm các trường dữ liệu khác trong mapping.
7. **Kiểm tra tài khoản** đảm bảo tài khoản Google Forms của bạn vẫn hoạt động.

{% hint style="info" %}
**Lưu ý:**

* Nêú  biểu mẫu của bạn có lựa chọn các giá trị ngày tháng và khách hàng của bạn ở ngoài Việt Nam, bạn cần tạo 1 lựa chọn múi giờ có các giá trị múi giờ như: +7, -7, +1, -1 .... để đảm bảo thời gian khách hàng chọn sẽ đúng múi giờ với bạn.
* Hệ thống mặc định múi giờ GTM+7 với các dữ liệu từ google form.
{% endhint %}

Để tùy chỉnh múi giờ trên Google Form, bạn cần có 1 trường dữ liệu mapping như hình dưới đây.

<figure><img src="../../../.gitbook/assets/image (721).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (722).png" alt="" width="426"><figcaption></figcaption></figure>

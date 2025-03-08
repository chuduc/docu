---
description: Hướng dẫn thiết lập gửi tin nhắn Messenger
---

# Messenger

Hệ thống gửi tin nhắn qua Messenger thông qua tài khoản Page Facebook bạn đã cấu hình. Chỉ gửi được tin nhắn với những người đã từng tương tác với Page đó.

1. Chọn loại nội dung tin nhắn:

* **Mặc định (Tin nhắn trong vòng 24 giờ):** Người nhận tin nhắn phải gửi tin nhắn cho Trang của bạn trong vòng 24 giờ qua hoặc đồng ý nhận tin nhắn từ Trang của bạn ngoài khoảng thời gian nhắn tin tiêu chuẩn 24 giờ.
* **Sự kiện cập nhật**: Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là lời nhắc cho sự kiện sắp tới hoặc thông tin cập nhật về sự kiện đang diễn ra mà khách hàng đã đăng ký.
* **Cập nhật thanh toán:** Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là thông tin cập nhật về giao dịch mua gần đây của khách hàng.
* **Cập nhật tài khoản:** Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là thông tin cập nhật không định kỳ về ứng dụng hoặc tài khoản của họ.

Xem thêm về các loại nội dung tin nhắn và cách sử dụng tại [phan-biet-cac-loai-tin-nhan-messenger.md](../../meo-su-dung-ladiflow/phan-biet-cac-loai-tin-nhan-messenger.md "mention")

3. **Điền nội dung tin nhắn.** Bạn có thể gắn biến dữ liệu của khách hàng bằng cách gõ \{{ và chọn trường thông tin tương ứng. Ví dụ tôi gửi nội dung tin nhắn khi khách hàng nhắn có chứa tên khách hàng như sau.

<figure><img src="../../.gitbook/assets/image (519).png" alt=""><figcaption></figcaption></figure>

Sẽ được kết quả như sau:

<figure><img src="../../.gitbook/assets/image (521).png" alt=""><figcaption></figcaption></figure>

4. **Chọn Thêm nút mới để thêm nút** cho tin nhắn.&#x20;
5. Điền tên và chọn hành động với từng nút.
6. Chọn Trả lời nhanh để thêm các nút cho khách hàng trả lời nhanh. Ví dụ như hình dưới đây:

<figure><img src="../../.gitbook/assets/image (460).png" alt=""><figcaption></figcaption></figure>

7. Chọn Flow tương ứng với từng nút bằng cách click vào nút đó, Flow phải được xuất bản. Kết quả sẽ như sau:

<figure><img src="../../.gitbook/assets/quick reply.png" alt=""><figcaption></figcaption></figure>

8. **Thêm các tin nhắn khác nếu muốn**. Bạn có thể tuỳ chỉnh nội dung tin nhắn: văn bản, video, hình ảnh, audio, file....

<figure><img src="../../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

* Văn bản: **tối đa 640 ký tự.**
* Hình ảnh: **Tối đa 1MB**, chấp nhận loại file **.png, .jpg,** .**jpeg, .gif, .svg,.ico**
* Bộ sưu tập: **Tối đa 10 ảnh, 1 MB/ảnh**, chấp nhận file **.png, .jpg,** .**jpeg, .gif, .svg, .ico**
* Video: **Tối đa 5MB**, chấp nhận file .**mp4**
* File: **Tối đa 5 MB**,  chấp nhận file  **.ttf, .otf, .woff2, .txt, .doc, .docx, .xls, .xlsx, .pdf**
* Delay: là hiệu ứng đang gõ, **tối đa 60 giây**
* Audio: **Tối đa 5MB**, chấp nhận file **.mp3**
* User input: lưu dữ liệu khách hàng nhập vào thông tin của khách hàng

9. **Chọn hành động khi gửi tin nhắn thành công, thất bại.** Dựa vào kết quả gửi tin, hệ thống sẽ chạy hành động tương ứng.&#x20;
10. Chọn các thông tin cho hành động ở bước 9 nếu có.
11. **Chọn tài khoản Facebook cấu hình.**
12. Chọn kiểm tra để kiểm tra tin nhắn của bạn. Chọn tài khoản và chọn Send to messenger để gửi tin nhắn kiểm tra.

**Lưu ý:**&#x20;

* Hành động gửi tin nhắn Messenger chỉ hoạt động được với những khách hàng tương tác với page đó trong tập khách hàng của bạn.

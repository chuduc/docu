# Gửi tin Messenger

Hệ thống gửi tin nhắn qua Messenger thông qua tài khoản Page Facebook bạn đã cấu hình. Với các trigger của Facebook, chỉ gửi được tin nhắn với những người đã từng tương tác với Page đó.

{% hint style="info" %}
Hành động gửi tin Messenger chỉ thực hiện được nếu khách hàng đã có tương tác với Facebook Page cài đặt trong Trigger.
{% endhint %}

Bạn phải chọn tài khoản page Facebook cấu hình tại các Trigger đang có. Nếu chưa có tài khoản hãy tích hợp thêm.

1. Chọn **+Thêm hành động**, tìm và chọn hành động **Gửi tin Messenger**

<figure><img src="../../../.gitbook/assets/gửi tin mess.png" alt=""><figcaption></figcaption></figure>

2. **Chọn loại nội dung tin nhắn**

* **Mặc định (Tin nhắn trong vòng 24 giờ):** Người nhận tin nhắn phải gửi tin nhắn cho Trang của bạn trong vòng 24 giờ qua hoặc đồng ý nhận tin nhắn từ Trang của bạn ngoài khoảng thời gian nhắn tin tiêu chuẩn 24 giờ.
* **Sự kiện cập nhật**: Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là lời nhắc cho sự kiện sắp tới hoặc thông tin cập nhật về sự kiện đang diễn ra mà khách hàng đã đăng ký.
* **Cập nhật thanh toán:** Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là thông tin cập nhật về giao dịch mua gần đây của khách hàng.
* **Cập nhật tài khoản:** Gắn thẻ tin nhắn bạn đang gửi cho khách hàng là thông tin cập nhật không định kỳ về ứng dụng hoặc tài khoản của họ.

Xem thêm về các loại nội dung tin nhắn và cách sử dụng tại [phan-biet-cac-loai-tin-nhan-messenger.md](../../../meo-su-dung-ladiflow/phan-biet-cac-loai-tin-nhan-messenger.md "mention")

3. **Điền nội dung tin nhắn**. Bạn có thể gắn biến dữ liệu của khách hàng bằng cách gõ \{{ và chọn trường thông tin tương ứng. Ví dụ tôi gửi nội dung tin nhắn khi khách hàng nhắn có chứa tên khách hàng như sau:

<figure><img src="../../../.gitbook/assets/image (519).png" alt=""><figcaption></figcaption></figure>

Sẽ được kết quả như sau

<figure><img src="../../../.gitbook/assets/image (521).png" alt=""><figcaption></figcaption></figure>

4. **Chọn Thêm nút mới để thêm nút cho tin nhắn**.&#x20;
5. **Điền tên và chọn hành động với từng nút**. Để điều hướng sang tin nhắn khác chọn Chuyển hướng, xem thêm tại [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")
6. **Chọn Trả lời nhanh để thêm các nút cho khách hàng trả lời nhanh.** Ví dụ như hình dưới đây:

<figure><img src="../../../.gitbook/assets/image (460).png" alt=""><figcaption></figcaption></figure>

7. Chọn hành động tương ứng với từng nút bằng cách click vào nút đó. Kết quả sẽ như sau:

<figure><img src="../../../.gitbook/assets/quick reply.png" alt=""><figcaption></figcaption></figure>

8. Thêm các tin nhắn khác nếu muốn. Bạn có thể tuỳ chỉnh nội dung tin nhắn: văn bản, video, hình ảnh, audio, file....

<figure><img src="../../../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

* Văn bản: **tối đa 640 ký tự.**
* Hình ảnh: **Tối đa 1MB**, chấp nhận loại file **.png, .jpg,** .**jpeg, .gif, .svg, .ico**
* Bộ sưu tập: **Tối đa 10 ảnh, 1 MB/ảnh**, chấp nhận file **.png, .jpg,** .**jpeg, .gif, .svg, .ico**
* Video: **Tối đa 5MB**, chấp nhận file .**mp4**
* File: **Tối đa 5 MB**,  chấp nhận file **.ttf, .otf, .woff2, .txt, .doc, .docx, .xls, .xlsx, .pdf**
* Delay: là hiệu ứng đang gõ, **tối đa 60 giây**
* Audio: **Tối đa 5MB**, chấp nhận file **.mp3**
* User input: lưu dữ liệu khách hàng nhập vào thông tin của khách hàng.

{% hint style="info" %}
Tối đa 1 hành động gửi Messenger có 10 tin nhắn. LadiFlow sẽ tính điểm theo từng tin nhắn trong hành động.
{% endhint %}

9. Chọn hành động khi gửi tin nhắn thành công, thất bại. Dựa vào kết quả gửi tin, hệ thống sẽ chạy hành động tương ứng. Cách làm tương tự như thêm nút.
10. **Mở chi tiết từng Trigger trong Flow,** **Chọn tài khoản Page Facebook cấu hình.**\


    <figure><img src="../../../.gitbook/assets/image (733).png" alt="" width="421"><figcaption></figcaption></figure>

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

**Lưu ý:**&#x20;

* Nội dung trong hành động, hệ thống tự động lưu sau khi bạn nhập vào.
* Nội dung tại Trigger, bạn cần chọn Lưu Trigger để lưu lại thông tin.
* Hành động gửi tin nhắn Messenger chỉ hoạt động được với những khách hàng tương tác với page đó trong tập khách hàng của bạn.

#### Hướng dẫn sử dụng nội dung User input messenger

1.  Chọn nội dung User Input\


    <figure><img src="../../../.gitbook/assets/image (588).png" alt=""><figcaption></figcaption></figure>
2.  Nhập nội dung câu hỏi hoặc yêu cầu để khách hàng của bạn trả lời. \


    <figure><img src="../../../.gitbook/assets/image (589).png" alt=""><figcaption></figcaption></figure>
3. Chọn kiểu văn bản trả lời. Đây là loại dữ liệu khách hàng sẽ nhập, hệ thống dựa vào loại dữ liệu này để xác minh dữ liệu khách hàng nhập đã đúng định dạng chưa.
   * Văn bản
   * Số
   * Gửi Email
   * Số điện thoại
4. Chọn trường tuỳ chỉnh lưu dữ liệu khách hàng nhập nếu muốn
5.  Chọn hành động nếu khách hàng phản hồi( điều kiện dữ liệu khách hàng nhập đã chính xác)\


    <figure><img src="../../../.gitbook/assets/image (591).png" alt=""><figcaption></figcaption></figure>
6.  Chọn thời gian hết hạn của User Input. Nếu sau khoảng thời gian này mà khách hàng chưa trả lời, User input sẽ hết hiệu lực. \


    <figure><img src="../../../.gitbook/assets/image (590).png" alt="" width="185"><figcaption></figcaption></figure>
7.  Chọn hành động nếu User input hết hạn và khách hàng không phản hồi. Hành động sẽ được thực hiện nếu quá thời gian hiệu lực của User input và trong suốt khoảng thời gian hiệu lực của User input khách hàng không phản hồi.\


    <figure><img src="../../../.gitbook/assets/image (592).png" alt=""><figcaption></figcaption></figure>
8. Chọn số lần thử lại khi khách hàng nhập dữ liệu không đúng định dạng đã cài đặt ở bước 3. Nếu số lần khách hàng nhập sai dữ liệu vượt quá con số này, hệ thống sẽ thực hiện hành động tiếp theo đã gắn với tin nhắn này( nếu có).

# Gửi mail

### Thêm hành động gửi mail vào Flow

1. Chọn **+ Thêm hành động,** tìm và chọn hành động **Gửi mail.**
2. **Nhập nội dung email**
   1. Nhập tiêu đề email.
   2. Nhập Preheader nếu có.
   3. Chọn mở trình thiết kế email để nhập nội dung. Có 2 chế độ thiết kế email: Classic editor, New editor.
   4. Thêm file đính kèm nếu có.
   5. Thêm hành động bổ sung: khi gửi tin thành công, khi gửi tin thất bại, hành động khi mở email, hành động khi click vào liên kết.
3. **Chọn tài khoản cấu hình gửi email.** Nếu chưa có tài khoản bạn có thể kết nối tài khoản mới.
4. Chọn mục kiểm tra, nhập email để nhận email kiểm tra nội dung email.

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

**Lưu ý:** Chỉ gửi được email với những khách hàng có thông tin email đúng, với những thông tin email sai sẽ tính vào số lượng Email bounce được hệ thống tổng hợp.

### Thiết kế email với Classic editor

Chọn **Classic Editor** sau đó chọn **Xác nhận**.\


<figure><img src="../../../.gitbook/assets/image (607).png" alt=""><figcaption></figcaption></figure>

Thanh công cụ giúp bạn dễ dàng soạn thảo văn bản. LadiFlow cung cấp các tác vụ soạn thảo văn bản cơ bản như khi bạn dùng trên Word.

Bạn có thể tải file HTML của bạn lên bằng cách chọn icon tải file HTML như hình. File tối đa **3000 ký tự.**

<figure><img src="../../../.gitbook/assets/tải html.png" alt=""><figcaption></figcaption></figure>

**Chọn OK** để lưu lại nội dung email..

### Thiết kế email với New editor

Chọn **New Editor** và chọn **Xác nhận** để bắt đầu sử dụng \


<figure><img src="../../../.gitbook/assets/image (608).png" alt=""><figcaption></figcaption></figure>

Kéo thả các nội dung bên trái vào nội dung chỉnh sửa để thiết kế email của bạn. Với trình thiết kế email này, bạn có thể tự do sáng tạo email.

<figure><img src="../../../.gitbook/assets/2023-09-26_10-29-32.gif" alt=""><figcaption></figcaption></figure>

Lưu mẫu email để tái sử dụng cho những lần tiếp theo.

**Chọn Cập nhật** để sử dụng nội dung email đã tạo.

**Lưu ý**: Nếu khách hàng xác nhận email của bạn là Spam, hệ thống sẽ không gửi email cho khách hàng đó nữa trên trên tất cả các tính năng.

### Nhập file email

LadiFlow cung cấp cho bạn 2 file nhập: HTML và  emailldf. Hệ thống tự động chọn ra trình thiết kế email tương ứng với file bạn tải lên.

#### HTML

Hiện nay trên thị trường có rất nhiều công cụ, mẫu email html, bạn chỉ cần tải xuống sau đó nhập trên hệ thống.&#x20;

<figure><img src="../../../.gitbook/assets/image (609).png" alt="" width="563"><figcaption></figcaption></figure>

Hệ thống sẽ tự động chọn trình thiết kế email classic để thuận tiện cho việc chỉnh sửa nội dung file.

#### emailldf

File .emailldf là file giao diện email do trình thiết kế New Editor cung cấp. Bạn chỉ có thể tải file .emailldf khi sử dụng trình thiết kế email New Editor

Để tải xuống file .**emailldf** bạn làm như sau:

**Chọn Mẫu,** sau đó tìm và chọn mẫu email muốn tải xuống. **Chọn xuất file .emailldf**

<figure><img src="../../../.gitbook/assets/image (610).png" alt="" width="563"><figcaption></figcaption></figure>

Ngoài ra, bạn có thế xuất file emailldf trên bản thiết kế email đang chỉnh sửa bằng cách chọn Nhập/Xuất file, sau đó chọn Xuất file. File .**emailldf** sẽ tải xuống thiết bị của bạn.

Vời file đã tải xuống, bạn có thể nhập file lên, **hệ thống sẽ hiển thị dữ liệu trên file thay thế dữ liệu đang có trên trình thiết kế email.**

### Kết nối tài khoản gửi email mới

**Cách 1:** Truy cập vào mục Tích hợp, chọn Dịch vụ Email và thêm mới liên kết.

**Cách 2:**&#x20;

1. Tại chi tiết hành động gửi email, chọn mục Chọn tài khoản.
2. Chọn Kết nối tài khoản mới.

Sau đó điền nội dung vào form thông tin yêu cầu và chọn **Lưu liên kết**.

**Lưu ý:**&#x20;

* Với những kết nối tài khoản mới, hệ thống sẽ gửi email xác thực, bạn cần phải xác thực email trước khi có thể sử dụng.
* Địa chỉ liên hệ bắt buộc nội dung: địa chỉ, số điện thoại.

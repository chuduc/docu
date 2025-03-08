# Nhập/xuất file dữ liệu khách hàng

### Nhập file Khách hàng

Nếu bạn đã có tập khách hàng, chỉ cần nhập file LadiFlow sẽ tự động thêm dữ liệu khách hàng.

1.  Chọn **Nhập/Xuất dữ liệu**, sau đó chọn **Nhập dữ liệu**.\


    <figure><img src="../../.gitbook/assets/image (734).png" alt=""><figcaption></figcaption></figure>
2. **Chọn và Tải file dữ liệu** lên hệ thống.

<figure><img src="../../.gitbook/assets/image (62).png" alt="" width="563"><figcaption></figcaption></figure>

Nếu bạn chưa biết file mẫu, hãy tải xuống file mẫu để xem.\


<figure><img src="../../.gitbook/assets/image (64).png" alt="" width="563"><figcaption></figcaption></figure>

**Lưu ý**:

* &#x20;Hệ thống chỉ chấp nhận đuôi file .xls, .xlsx.
* Số lượng khách hàng tối đa 1 lần nhập là 30.000 khách hàng
* Dung lượng file tối đa 80MB
* File tải lên không cần giống chính xác file mẫu nhưng phải có ít nhất 1 cột dữ liệu **email** hoặc **phone**.

3. Nếu bạn **KHÔNG muốn cập nhật dữ liệu của khách hàng đã có nếu có dữ liệu trong file nhập tồn tại email của khách hàng** **đó,** bạn hãy **bỏ chọn** **Cập nhật thông tin khách hàng trên hệ thống có cùng địa chỉ email**.&#x20;

<figure><img src="../../.gitbook/assets/image (65).png" alt="" width="563"><figcaption></figcaption></figure>

Ngược lại, nếu tích chọn dữ liệu khách hàng sẽ được cập nhật theo file nếu đã tồn tại khách hàng trên hệ thống.

4. Nếu bạn muốn thực hiện chạy kịch bản tự động - Flow với các khách hàng được cập nhật/thêm mới bằng hình thức nhập file dữ liệu, hãy chọn **Thực hiện các kịch bản flow liên quan.**\
   **Lưu ý: Chỉ thực hiện Flow liên quan nếu khách hàng thỏa mãn các trigger đã kích hoạt trong Flow tương ứng.**\
   &#x20;Các Flow liên quan bao gồm các flow có các trigger liên quan đến dữ liệu khách hàng thay đổi:  Trường tùy chỉnh thay đổi, Trường mặc định thay đổi, Điểm khách hàng thay đổi, Đăng ký mới,...

<figure><img src="../../.gitbook/assets/image (66).png" alt="" width="563"><figcaption></figcaption></figure>

5. **Chọn Xác nhận** để hệ thống tiến hành nhập dữ liệu.

Nếu file nhập được hệ thống xác định hợp lệ, bạn sẽ thấy 1 tiến trình nhập file tại góc phải dưới màn hình.

<figure><img src="../../.gitbook/assets/image (67).png" alt="" width="563"><figcaption></figcaption></figure>

&#x20;**Sau khi tiến trình hoàn tất sẽ có thể xảy ra 2 trường hợp sau**:

**Trường hợp 1**: **Nhập file hoàn thành**: toàn bộ dữ liệu khách hàng trong file đã được tạo mới/ cập nhật thành công\


<figure><img src="../../.gitbook/assets/image (69).png" alt="" width="563"><figcaption></figcaption></figure>

**Trường hợp 2**: **Nhập file hoàn tất**: trong file nhập có chứa dữ liệu không hợp lệ, các khách hàng hợp lệ đã được thêm trên hệ thống thành công.

* Hệ thống sẽ gửi email cho bạn thông báo số khách hàng được cập nhật/thêm mới thành công, danh sách khách hàng không hợp lệ và các lỗi của khách hàng đó.
*   Bạn có thể tải xuống danh sách khách hàng không hợp lệ đồng thời mở xem danh sách lỗi của các khách hàng này. Bạn có thể sửa lại nội dung của các khách hàng không hợp lệ này theo lỗi hệ thống trả về và nhập lại trên hệ thống nếu muốn.\


    <figure><img src="../../.gitbook/assets/image (616).png" alt="" width="563"><figcaption></figcaption></figure>

Ngoài ra, nếu dữ liệu trong file nhập của bạn không hợp lệ bất cứ thông tin nào ngoài Email và Số điện thoại, chỉ thông tin đó sẽ không được cập nhật vào khách hàng, các thông tin hợp lệ vẫn sẽ được cập nhật trên hệ thống. \
Ví dụ, với cột dữ liệu **gender** bạn điền trong file là NAM và hệ thống chỉ chấp nhận một trong 2 giá trị: Nam hoặc Nữ, thì dữ liệu gender = NAM sẽ không được cập nhật trên các khách hàng.

Sau khi nhập file hoàn thành, hệ thống sẽ gửi mail cho bạn thông báo kết quả nhập dữ liệu. Bạn hoàn toàn có thể xem lại các dữ liệu lỗi và các lỗi nếu có.



### Xuất file khách hàng

<figure><img src="../../.gitbook/assets/image (741).png" alt=""><figcaption></figcaption></figure>

LadiFlow cho phép bạn và doanh nghiệp xuất file Excel danh sách khách hàng nhanh chóng:

* Xuất toàn bộ khách hàng trên trang hiện tại
* Xuất tất cả các khách hàng mà bạn có (không áp dụng bộ lọc nâng cao)
* Chỉ xuất các khách hàng bạn đã chọn
* Chỉ xuất các khách hàng phù hợp với bộ lọc đang áp dụng.

Nếu dữ liệu xuất **không dưới 10.000** khách hàng thì file dữ liệu sẽ được tải xuống thiết bị của bạn ngay khi hoàn thành.

Nếu dữ liệu xuất trên **10.000** khách hàng thì hệ thống sẽ gửi email cho bạn danh sách file dữ liệu. Mỗi file tối đa **30.000 khách hàng.**

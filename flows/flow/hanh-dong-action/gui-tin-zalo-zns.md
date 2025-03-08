# Gửi tin Zalo ZNS

Dịch vụ Zalo ZNS cho phép doanh nghiệp quản lý các mẫu thông báo của OA và tương tác với khách hàng thông qua số điện thoại liên kết với tài khoản Zalo sử dụng các mẫu thông báo mà bạn đã đăng ký với Zalo. Nếu bạn chưa có bất kỳ mẫu ZNS nào, liên hệ với CSKH để đăng ký.

{% hint style="info" %}
Hành động có thể thực hiện được nếu có dữ liệu số điện thoại khách hàng kích hoạt trigger và khách hàng đã có tài khoản Zalo.

Thời gian gửi tin 6h->21h59
{% endhint %}

1. Chọn **+Thêm hành động,** tìm và **chọn Gửi tin Zalo ZNS.**

<figure><img src="../../../.gitbook/assets/zalo zns.png" alt=""><figcaption></figcaption></figure>

2. **Chọn mẫu tin ZNS**. Nếu bạn chưa có tin nhắn mẫu nào, hãy liên hệ CSKH của LadiFlow để đăng ký.

{% hint style="info" %}
Với mỗi mẫu tin nhắn khác nhau, Zalo sẽ yêu cầu các thông tin khác nhau.
{% endhint %}

3.  **Điền nội dung thiết lập tin nhắn** bằng cách chọn các trường thông tin trên LadiFlow tương ứng với các nội dung Zalo yêu cầu.\
    \- Để chọn các trường thông tin cá nhân hóa theo khách hàng, bạn chọn vào biểu tượng Cá nhân hóa, tìm chọn trường thông tin mong muốn.\


    <figure><img src="../../../.gitbook/assets/image (745).png" alt="" width="426"><figcaption></figcaption></figure>

&#x20;\- Để nhập giá trị mặc định cho tham số, bạn nhập giá trị mặc định vào ô Nhập giá trị tương ứng với tham số\


<figure><img src="../../../.gitbook/assets/image (746).png" alt="" width="436"><figcaption></figcaption></figure>

4. **Nếu mẫu tin bạn chọn là mẫu tin đánh giá dịch vụ**, bạn có thể tùy chỉnh dữ liệu báo cáo bằng cách chọn **Thêm dữ liệu báo cáo bổ sung**

<figure><img src="../../../.gitbook/assets/image (748).png" alt="" width="434"><figcaption></figcaption></figure>

{% hint style="info" %}
Các dữ liệu báo cáo bổ sung này sẽ hiển thị khi bạn chọn Xem đánh giá khách hàng.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (749).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (750).png" alt="" width="563"><figcaption></figcaption></figure>

5. **Chọn các hành động bổ sung**: hành động khi gửi tin thành công, hành động khi gửi tin thất bại.\
   \


<figure><img src="../../../.gitbook/assets/image (747).png" alt="" width="431"><figcaption></figcaption></figure>

6. **Chọn tài khoản Zalo OA** thực hiện hành động. Nếu bạn chưa có bạn có thể chọn Kết nối tài khoản mới, xem thêm tại [tich-hop-zalo.md](../../../tich-hop/huong-dan-tich-hop/tich-hop-zalo.md "mention").

<figure><img src="../../../.gitbook/assets/image (229).png" alt="" width="321"><figcaption><p>Tích hợp Zalo còn hiệu lực</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (224).png" alt="" width="323"><figcaption><p>Tích hợp Zalo còn hiệu lực dưới 10 ngày</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (225).png" alt="" width="319"><figcaption><p>Tích hợp Zalo đã hết hạn</p></figcaption></figure>

Nếu tích hợp Zalo hết hạn, bạn cần thao tác đăng nhập lại tài khoản.

7. Kiểm tra nội dung tin nhắn để đảm bảo tin nhắn được gửi thành công

{% hint style="info" %}
**Để đảm bảo tin ZNS gửi thành công ngoài trước 6h và sau 21h59, bạn hãy đặt thêm 1 hành động Hẹn giờ ngay trước khi gửi tin ZNS và cài đặt như hình sau**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (283).png" alt="" width="321"><figcaption></figcaption></figure>

**Lưu ý**:&#x20;

* Gửi tin nhắn zalo ZNS chỉ gửi được nếu thông tin số điện thoại của khách hàng chính xác và số điện thoại đã có tài khoản zalo.
* Nội dung thiếp lập tin nhắn đúng theo định dạng yêu cầu của mẫu bạn đã chọn. Nếu không việc gửi tin Zalo ZNS sẽ thất bại.
* Nên kiểm tra tin ZNS để đảm bảo dữ liệu thiết lập đã chính xác.

**Một số lỗi phổ biến khi gửi thất bại tin ZNS**:

* **Thiết lập sai dữ liệu so với thông tin đăng ký mẫu ZNS**: ví dụ bạn đăng ký mẫu ZNS  với trường kiểu số, nhưng dữ liệu bạn điền thông tin trong mẫu tin lại là trường tùy chỉnh thuộc loại Dòng văn bản. Sự khác biệt về loại dữ liệu khiến tin ZNS của bạn thất bại.
* **Dữ liệu sai định dạng của mẫu tin**: ví dụ mẫu ZNS đăng ký với trường kiểu số tự nhiên, nhưng dữ liệu của bạn lại là số thập phân.&#x20;
* **Dữ liệu quá ký tự cho phép**: ví dụ mẫu tin ZNS đăng ký có trường dữ liệu tối đa 30 ký tự, dữ liệu bạn chọn có nhiều hơn 30 ký tự. Đây là lỗi thường xuyên xảy ra.
* **Số điện thoại chưa đăng ký tài khoản Zalo**: khách hàng chưa có tài khoản Zalo sẽ không thể nhận tin nhắn ZNS

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

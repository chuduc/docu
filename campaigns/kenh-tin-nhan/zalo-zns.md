---
description: Hướng dẫn thiết lập gửi tin nhắn Zalo ZNS
---

# Zalo ZNS

Gửi tin nhắn Zalo ZNS thông qua tài khoản Zalo OA của bạn.

1. **Chọn tin nhắn mẫu**. Nếu bạn chưa có tin nhắn mẫu nào, hãy liên hệ CSKH để đăng ký.

{% hint style="info" %}
Với mỗi mẫu tin nhắn khác nhau, Zalo sẽ yêu cầu các thông tin khác nhau.

Bạn không thể tự tuỳ chỉnh tin nhắn, ví dụ thêm nút trong tin nhắn.

Thời gian gửi tin 6h->21h59
{% endhint %}

3.  **Điền nội dung thiết lập tin nhắn** bằng cách chọn các trường thông tin trên LadiFlow tương ứng với các nội dung Zalo yêu cầu.\
    \- Để chọn các trường thông tin cá nhân hóa theo khách hàng, bạn chọn vào biểu tượng Cá nhân hóa, tìm chọn trường thông tin mong muốn.\


    <figure><img src="../../.gitbook/assets/image (659).png" alt="" width="324"><figcaption><p><br></p></figcaption></figure>

    &#x20;\- Để nhập giá trị mặc định cho tham số, bạn nhập giá trị mặc định vào ô Nhập giá trị tương ứng với tham số\


    <figure><img src="../../.gitbook/assets/image (660).png" alt="" width="319"><figcaption></figcaption></figure>
4. **Nếu mẫu tin bạn chọn là mẫu tin đánh giá dịch vụ**, bạn có thể tùy chỉnh dữ liệu báo cáo bằng cách chọn **Thêm dữ liệu báo cáo bổ sung**

<figure><img src="../../.gitbook/assets/image (748).png" alt="" width="434"><figcaption></figcaption></figure>

{% hint style="info" %}
Các dữ liệu báo cáo bổ sung này sẽ hiển thị khi bạn chọn Xem đánh giá khách hàng.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (749).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (750).png" alt="" width="563"><figcaption></figcaption></figure>

5. **Chọn các hành động bổ sung**: hành động khi gửi tin thành công, hành động khi gửi tin thất bại.
6. **Chọn tài khoản Zalo OA** thực hiện hành động. Nếu bạn cha có bạn có thể chọn Kết nối tài khoản mới.
7. Chọn mục kiểm tra, nhập số điện thoại để nhận tin nhắn zalo bạn vừa thiết kế.

{% hint style="info" %}
**Để đảm bảo tin ZNS gửi thành công ngoài trước 6h và sau 21h59, bạn hãy đặt thêm 1 hành động Hẹn giờ ngay trước khi gửi tin ZNS và cài đặt như hình sau**


{% endhint %}

<figure><img src="../../.gitbook/assets/image (283).png" alt="" width="321"><figcaption></figcaption></figure>

**Lưu ý**:&#x20;

* Gửi tin nhắn zalo ZNS chỉ gửi được nếu thông tin số điện thoại của khách hàng chính xác và số điện thoại đã có tài khoản zalo.
* Nội dung thiếp lập tin nhắn đúng theo định dạng yêu cầu của mẫu bạn đã chọn. Nếu không việc gửi tin Zalo ZNS sẽ thất bại.
* Nên kiểm tra tin ZNS để đảm bảo dữ liệu thiết lập đã chính xác.

**Một số lỗi phổ biến khi gửi thất bại tin ZNS:**

* **Thiết lập sai dữ liệu so với thông tin đăng ký mẫu ZNS**: ví dụ bạn đăng ký mẫu ZNS  với trường kiểu số, nhưng dữ liệu bạn điền thông tin trong mẫu tin lại là trường tùy chỉnh thuộc loại Dòng văn bản. Sự khác biệt về loại dữ liệu khiến tin ZNS của bạn thất bại.
* **Dữ liệu sai định dạng của mẫu tin**: ví dụ mẫu ZNS đăng ký với trường kiểu số tự nhiên, nhưng dữ liệu của bạn lại là số thập phân.&#x20;
* **Dữ liệu quá ký tự cho phép**: ví dụ mẫu tin ZNS đăng ký có trường dữ liệu tối đa 30 ký tự, dữ liệu bạn chọn có nhiều hơn 30 ký tự. Đây là lỗi thường xuyên xảy ra.
* **Số điện thoại chưa đăng ký tài khoản Zalo:** khách hàng chưa có tài khoản Zalo sẽ không thể nhận tin nhắn ZNS

{% hint style="info" %}
Bạn nên thực hiện kiểm tra ZNS và chạy thử dữ liệu với dữ liệu cá nhân trước khi áp dụng cho toàn bộ tập khách hàng để phát hiện và sửa lỗi kịp thời. Ngoài ra, đảm bảo các khách hàng có dữ liệu cá nhân hóa đúng định dạng thỏa mãn mẫu tin đã đăng ký.
{% endhint %}

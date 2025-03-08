# Chỉnh sửa dữ liệu trang tính Google sheet( tự động)

Trigger này được kích hoạt khi trang tính được cập nhật thủ công, tự động. Với trigger mới này, bạn chỉ cần thao tác đơn giản trên LadiFlow, kịch bản sẽ tự động thực hiện với các khách hàng thay đổi trên trang tính của bạn.&#x20;

{% hint style="info" %}
**Lưu ý**:&#x20;

* Trang tính của bạn bắt buộc phải có cột thông tin Email hoặc số điện thoại của khách hàng.
* &#x20;Hệ thống sẽ dựa theo thông tin email, số điện thoại tại hàng có ô tính được chỉnh sửa dữ liệu để thực hiện các hành động với khách hàng đó.


{% endhint %}

**Gợi ý các hành động phù hợp với các trigger**:&#x20;

* Các hành động trên LadiFlow: gắn tag, đăng ký sequence...&#x20;
* Gửi Email nếu đã có thông tin địa chỉ email (đã xác thực) tại hàng có ô tính thay đổi.&#x20;
* Gửi SMS, Zalo ZNS, AI call nếu đã có thông tin số điện thoại tại hàng có ô tính thay đổi.&#x20;
* Messenger nếu khách hàng của bạn đã/đang tương tác với bạn qua Messenger.
* Gửi thông báo Telegram, Slack, Email.

### **Các bước thiết lập như sau**:&#x20;

1.  Chọn **Trigger Hàng tính được tạo mới hoặc chỉnh sửa (Tự động)**\


    <figure><img src="../../../.gitbook/assets/image (725).png" alt="" width="311"><figcaption></figcaption></figure>
2. Chọn **tài khoản Google Sheet tích hợp**. Đây là tài khoản chứa trang tính của bạn, nếu bạn chưa có tài khoản nào hãy tích hợp thêm.&#x20;

<figure><img src="../../../.gitbook/assets/image (726).png" alt="" width="425"><figcaption></figcaption></figure>

1. Chọn mục Thiết lập Trigger, thêm điều kiện kích hoạt nếu muốn giới hạn tệp khách hàng trong flow. Xem thêm tại[them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
2.  **Chọn trang tính** **mà bạn muốn thực hiện Trigger**. \
    Bạn có thể tạo mới trang tính ngay trên LadiFlow với tài khoản Google Sheet đã tích hợp.\
    Bạn cũng có thể điền ID bảng tính thay vì điền tên. ID của bảng tính lấy dựa theo đường dẫn của bảng tính đó.\


    <figure><img src="../../../.gitbook/assets/id sheet.png" alt=""><figcaption><p>ID trang tính trên google sheet</p></figcaption></figure>
3.  **Chọn Sheet lấy dữ liệu**. Đây là Trang tính mọi sự thay đổi dữ liệu trên ô tính, hệ thống sẽ thực hiện cập nhật dữ liệu khách hàng tại hàng có ô tính thay đổi dữ liệu. \


    <figure><img src="../../../.gitbook/assets/image (727).png" alt="" width="429"><figcaption></figcaption></figure>
4.  **Chọn Cột tính thay đổi dữ liệu ( không bắt buộc)**\
    Nếu bạn chọn cột tính, chỉ khi dữ liệu thay đổi tại cột đã chọn thì Trigger mới được chạy. Nếu bạn không chọn cột tính, bất kì sự thay đổi tại bất kỳ ô tính nào Trigger cũng chạy. \


    <figure><img src="../../../.gitbook/assets/image (728).png" alt="" width="428"><figcaption></figcaption></figure>
5. **Điền thông tin mapping dữ liệu**. \
   Bên phải là trường dữ liệu của khách hàng trên LadiFlow, bên trái là các cột lấy dữ liệu tương ứng.&#x20;

{% hint style="info" %}
* Hệ thống tự động lấy hàng 1 trên sheet để làm dữ liệu mapping.&#x20;
* Dữ liệu mapping phải có dữ liệu số điện thoại hoặc email thì mới thực hiện hành động trong Flow.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (729).png" alt="" width="427"><figcaption></figcaption></figure>

8. Kiểm tra tài khoản đảm bảo tài khoản google sheet của bạn vẫn đang hoạt động.

### Các lưu ý khi sử dụng Trigger Hàng tính được tạo mới hoặc chỉnh sửa (Tự động) của Google Sheet&#x20;

#### Tên trang tính( Sheet) và file dữ liệu&#x20;

* Không được chứa ký tự cách tại vị trí đầu và cuối.&#x20;
* Không được chứa các ký tự đặc biệt.
* Dòng đầu tiên trong file để tiêu đề dữ liệu LadiFlow sẽ dựa vào dòng đầu tiên trong file để xác định tiêu đề các cột, do đó bạn bắt buộc phải thiết lập tiêu đề vào dòng đầu tiên trước khi thiết lập file đó trên trigger của LadiFlow.&#x20;
* Không đặt tên tiêu đề các cột trùng nhau, điều này dẫn tới việc xác định, tính toán gặp sai và gây lỗi.
* &#x20;Cột tính với tiêu đề trống không thể dùng để mapping dữ liệu lên LadiFlow

#### Thay đổi nội dung dữ liệu trong trang tính đã thiết lập&#x20;

Nếu bạn muốn thay đổi nội dung dữ liệu trong sheet sau khi **Trigger đã kích hoạt** bao gồm các hành động sau:

* &#x20;Thay đổi tên Trang tính&#x20;
* Thay đổi tên file google sheet&#x20;
* Thay đổi tên tiêu đề cột
* &#x20;Xóa tiêu đề cột&#x20;
* Thay đổi vị trí các cột
* &#x20;Chèn thêm 1 cột vào giữa các cột đã mapping dữ liệu&#x20;

Thì bạn cần thực hiện các hành động sau trước khi thực hiện thay đổi trên file google sheet đã kết nối với LadiFlow&#x20;

1. Tắt kích hoạt trigger&#x20;
2. Thực hiện thay đổi trên file Sheet
3. Bật kích hoạt lại trigger

&#x20;Nếu bạn không thực hiện theo các bước ở trên, dữ liệu thực hiện trigger sẽ không đảm bảo tính chính xác và có thể xảy ra lỗi.&#x20;

#### Thời gian thực hiện kịch bản sau khi thay đổi trên file sheet

&#x20;Thời gian thực hiện kịch bản sau khi có sự thay đổi trên file sheet sẽ dao động từ 1 đến 5 phút phụ thuộc vào các yếu tố sau:

* &#x20;**Độ trễ mạng**: Thời gian để dữ liệu được truyền giữa máy chủ của Google và LadiFlow có thể thay đổi tùy thuộc vào tình trạng mạng.&#x20;
* **Tải máy chủ**: phụ thuộc vào tải máy chủ của Google.
* **Kích thước tệp**: Nếu tệp bạn đang thay đổi có kích thước lớn, thời gian để Google xử lý thay đổi và gửi thông báo cho LadiFlow sẽ lâu hơn.&#x20;
* **Số lượng thay đổi**: Nếu bạn thực hiện nhiều thay đổi vào tệp cùng một lúc, thời gian để Google xử lý tất cả các thay đổi và gửi thông báo cho LadiFlow có thể lâu hơn.&#x20;

#### Giới hạn về file google sheet : tối đa 10.000 dòng chứa dữ liệu trên file sheet

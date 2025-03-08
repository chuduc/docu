# Catch hook

Khi có dữ liệu từ Webhook từ bên khác gửi về LadiFlow bạn hãy cài đặt Trigger Catch hook.  Bạn hãy sử dụng trigger catch hook trong trường hợp: Dữ liệu từ đối tác chưa tích hợp LadiFlow, dữ liệu từ đối tác đã tích hợp với LadiFlow nhưng chưa đủ để xây dựng kịch bản... Để cài đặt Trigger Catch hook bạn làm như sau:

1. **Tìm và chọn thêm trigger Catch hook**
2. Chọn Kênh thiết lập Trigger **chọn kênh**\
   **- Kênh WPFORM7 :** form của bạn được thiết lập thuộc loại wpform 7 trên Woocomerce/ Wordpress\
   \- **Kênh WPFORMS:** form của bạn được thiết lập thuộc loại wpforms trên Woocomerce/ Wordpress\
   \- **Kênh GOOGLE LEAD ADS**: dữ liệu từ google lead ads \
   \- **Kênh OTHER:** Dữ liệu từ các kênh khác không liệt kê ở trên
3. Sao chép webhook URL để gửi hook. Lưu ý đường dẫn webhook phải gửi đúng theo thông tin của trigger thì Flow mới chạy. Với WPFORM7 và WPFORMS xem cách thiết lập Webhook url tại [#huong-dan-thiet-lap-webhook-url-tren-wordpress-woocomerce](catch-hook.md#huong-dan-thiet-lap-webhook-url-tren-wordpress-woocomerce "mention")
4.  Nếu bạn chọn kênh WPFORM7 hoặc WPFORMS, bạn cần chọn tích hợp Wordpress và Form tương ứng theo tài khoản\


    <figure><img src="../../../.gitbook/assets/image (652).png" alt="" width="317"><figcaption></figcaption></figure>
5.  **Điền/chọn các thông tin mapping lưu dữ liệu từ hook sang LadiFlow**

    Bên tay phải bạn chọn các trường dữ liệu của khách hàng lưu thông tin từ hook

    Bên tay trái bạn điền/chọn tên các params từ hook.\
    Với kênh WPFORM7 và WPFORMS, hệ thông cho phép bạn chọn các trường tương ứng trong form đã thiết lập. Với các kênh khác, bạn cần điền tên trường tương ứng vào thiết lập\
    Dưới đây là ví dụ với kênh OTHER\


<figure><img src="../../../.gitbook/assets/image (218).png" alt="" width="463"><figcaption></figcaption></figure>

Request gọi từ Postman tương ứng với thiết lập ở trên như sau:

<figure><img src="../../../.gitbook/assets/image (219).png" alt="" width="563"><figcaption></figcaption></figure>

**Lưu ý:** Để tiền tố **LF:** trước tên params nếu như dữ liệu Body gửi đi có dạng Object phức tạp. Ví dụ

<figure><img src="../../../.gitbook/assets/image (220).png" alt=""><figcaption></figcaption></figure>

Bạn sẽ cần thiết lập trên LadiFlow như sau:

<figure><img src="../../../.gitbook/assets/image (223).png" alt="" width="475"><figcaption></figcaption></figure>

LadiFlow hỗ trợ 2 phương thức: **GET và POST** để nhận hook.

{% hint style="info" %}
Bạn cần đảm bảo điền đúng chỉnh tả, không có các ký thừa. Chúng tôi khuyến cáo bạn nên đặt tên tham số không có dấu cách, dấu trong tiếng việt, ký tự đặc biệt.\
Ví dụ:

* &#x20;ho\_va\_ten => :white\_check\_mark:
* họ và tên => :x:
{% endhint %}

5. Sau khi điền đủ thông tin, thêm các hành động trong Flow, xuất bản Flow kèm kích hoạt trigger

### Hướng dẫn thiết lập Webhook URL trên Wordpress/Woocomerce

1. Truy cập vào LadiApp trên thanh menu

<figure><img src="../../../.gitbook/assets/image (653).png" alt="" width="563"><figcaption></figcaption></figure>

2. Mở tab LadiFlow
3. Điền Webhook URL đã sao chép tại màn hình thiết lập Trigger trên LadiFlow tương ứng với Form

<figure><img src="../../../.gitbook/assets/image (654).png" alt="" width="563"><figcaption></figcaption></figure>

4. Chọn **Save** để lưu lại thiết lập.

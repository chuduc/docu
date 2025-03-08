# Cơ chế trừ điểm, tiền trên LadiFlow

LadiFlow sẽ thực hiện trừ điểm trên tất cả các hành động trong Flow, Campaign, Sequence và thực hiện trừ tiền với tin Zalo, AI call. Bài viết này sẽ giúp bạn hiểu rõ chi tiết về cơ chế trừ điểm, tiền trên LadiFlow.

{% hint style="info" %}
Chi tiết bảng giá từng hành động bạn xem tại [bang-gia-chi-phi-va-gioi-han-he-thong.md](bang-gia-chi-phi-va-gioi-han-he-thong.md "mention")
{% endhint %}

{% hint style="info" %}
Để hiểu rõ quá trình gửi tin, thực hiện hành động bạn xem thêm tại [cac-trang-thai-gui-tin-tren-ladiflow.md](cac-trang-thai-gui-tin-tren-ladiflow.md "mention")
{% endhint %}

Tôi sẽ mô tả ngắn gọn quá trình gửi tin, thực hiện hành động trên LadiFlow như sau:

Bước 1: LadiFlow sẽ gửi yêu cầu( Request) sang bên thứ 3( Messenger, Zalo, eSMS, ...)

Bước 2: Bên thứ 3 thực hiện yêu cầu. Bên thứ 3 có thể từ chối yêu cầu nếu yêu cầu không hợp lệ

Bước 3: Tin nhắn, hành động được thực hiện với khách hàng. Bên thứ 3 gửi Thông báo gửi tin thành công về LadiFlow

Bước 4: Khách hàng mở tin, click vào đường dẫn, nút trong tin... bên thứ 3 gửi Thông báo về LadiFlow.

Hình dưới đây sẽ mô tả quá trình gửi tin Zalo trên LadiFlow.

<figure><img src="../.gitbook/assets/trạng thái gửi tin.drawio (1).png" alt=""><figcaption><p>Quá trình gửi tin Zalo từ LadiFlow</p></figcaption></figure>

Tại bước 2: **Nếu yêu cầu bị bên thứ 3 từ chối thì LadiFlow sẽ không trừ điểm/tiền với các lượt chạy này**. Các điều kiện phổ biến gửi tin mà bên thứ 3 yêu cầu:

* Độ dài tin: Độ dài tin phải thỏa mãn quy định. Nếu bạn sử dụng tính năng cá nhân hóa và dữ liệu cá nhân hóa theo khách hàng quá dài sẽ dẫn tới độ dài tin vượt quá quy định.
* &#x20;Các tham số: Các dữ liệu tham số phải đáp ứng quy định về độ dài dữ liệu, kiểu dữ liệu, format...
* Nội dung tin: Nội dung tin theo quy định của từng loại tin. Ví dụ tin SMS chứa các từ khóa quảng cáo, khuyến mại và bạn chọn loại tin chăm sóc khách hàng thì tin sẽ bị từ chối.
* Người nhận tin: Người nhận tin cần đáp ứng điều kiện nhận tin theo loại tin. Ví dụ tin Messenger mặc định 24h nhưng khách hàng không tương tác với page trong vòng 24h thì yêu cầu sẽ bị từ chối.
* ...

Tại bước 2: **Nếu yêu cầu được bên thứ 3 chấp nhận thì LadiFlow sẽ trừ điểm, tiền với các lượt chạy này**

* Tất cả các hành động đều bị trừ điểm, số điểm đã được quy định theo bảng giá.
* Các hành động trừ tiền: AI CALL, ZNS, Zalo Quan tâm
* Bên thứ 3 chấp nhận thì quá trình gửi tin sẽ phụ thuộc vào bên thứ 3. Nếu người nhận đã nhận được tin, LadiFlow sẽ nhận được tín hiệu từ bên thứ 3 và cập nhật dữ liệu báo cáo.

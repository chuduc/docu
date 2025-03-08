# Tự động đồng bộ CTKM từ CRM IPOS

Bạn chỉ cần tạo các Chương trình khuyến mại trên CRM IPOS, mã khuyến mại và Chương trình khuyến mại sẽ tự động tạo trên tài khoản LadiFlow của bạn tương ứng.

### Bật thiết lập đồng bộ CTKM từ CRM IPOS

Bạn cần bật thiết lập đồng bộ CTKM từ CRM IPOS trên tích hợp IPOS của bạn:

1. Chọn **Tích hợp** trên menu
2. Tìm và chọn tích hợp IPOS. **Bật Tự động đồng bộ CTKM từ CRM IPOS**

<figure><img src="../.gitbook/assets/image (777).png" alt="" width="563"><figcaption></figcaption></figure>

3. Chọn **Lưu liên kết**

### Thêm chương trình khuyến mại phát hành trên LadiPage

Chỉ chương trình khuyến mại phát hành trên kênh đối tác LadiPage mới có thể tự động đồng bộ sang LadiFlow. Bạn cần đảm bảo chương trình khuyến mại được tạo có:

* Mục đích: Phát hành trên kênh đối tác
* Kênh phân phối: LadiPage

<figure><img src="../.gitbook/assets/image (778).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (775).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
Chương trình khuyến mại sẽ tự động tạo trên tài khoản LadiFlow của bạn. Hệ thống lấy danh sách mã khuyến mại từ IPOS về trong khoảng 10 phút.
{% endhint %}

{% hint style="info" %}
Sau 10 phút, mã khuyến mại đã được kéo về LadiFlow đủ số lượng, bạn có thể bắt đầu chạy kịch bản phân phối các mã khuyến mại này.
{% endhint %}

**Lưu ý**:

*   Nếu quá trình đồng bộ CTKM (Chương trình khuyến mại) bị lỗi, chúng tôi sẽ gửi email tới hòm thư của bạn.&#x20;

    * Nếu lỗi trong quá trình tạo CTKM, bạn cần thao tác tạo lại CTKM trên CRM IPOS
    * Nếu lỗi trong quá trình kéo danh sách mã khuyến mại, bạn cần thao tác xuất file trên IPOS và nhập file mã vào CTKM trên LadiFlow
    * CTKM được tạo tự động sẽ có icon Đồng bộ như hình sau:

    <figure><img src="../.gitbook/assets/image (776).png" alt="" width="563"><figcaption></figcaption></figure>


* Chỉ CTKM tạo tự động, khi phân phối dữ liệu sẽ được đồng bộ sang IPOS. Nghĩa là, trên LadiFlow bạn phân phối cho ai thì trên IPOS sẽ có dữ liệu tương tự. Trong trường hợp khách hàng trên LadiFlow chưa có trên IPOS thì quá trình này sẽ không thể thực hiện được.

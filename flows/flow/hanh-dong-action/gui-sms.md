# Gửi SMS

Khi bạn muốn gửi tin nhắn SMS cho khách hàng của bạn, sử dụng hành động Gửi Sms.

{% hint style="info" %}
Hành động gửi tin nhắn SMS chỉ thực hiện được nếu khách hàng thực hiện Trigger có dữ liệu số điện thoại trên LadiFlow.
{% endhint %}

**Lưu ý:**

* **Để gửi được tin nhắn SMS, bạn phải tích hợp tài khoản eSMS.**
* **Tài khoản eSMS gửi tin phải có Brand name phải là CSKH**

1. Chọn +**Thêm hành động**, tìm và chọn hành động **Gửi SMS.**
2. **Nhập nội dung tin nhắn**. Số ký tự tối đa cho phép 640 ký tự. Bạn có thể gắn biến dữ liệu của khách hàng bằng cách gõ \{{ và chọn trường thông tin tương ứng.

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

4. Chọn thêm liên kết khi muốn thêm đường dẫn vào tin nhắn và hành động sau khi click vào đường dẫn.
5. Thêm hành động bổ sung: khi gửi tin thành công, gửi tin thất bại, khi khách hàng click vào link.
6. **Mở mục Chọn tài khoản, chọn tài khoản tích hợp gửi tin SMS.** Nếu bạn chưa có, hãy tích hợp thêm.
7. Mở mục kiểm tra, nhập số điện thoại để nhận tin nhắn kiểm tra trước khi xuất bản.

**Lưu ý:**&#x20;

* Dịch vụ SMS bạn sẽ phải trả phí theo số lượng tin. Tham khảo biểu phí tại [bang-gia-chi-phi-va-gioi-han-he-thong.md](../../../cai-dat/bang-gia-chi-phi-va-gioi-han-he-thong.md "mention").
* Với những khách hàng không có thông tin số điện thoại, số điện thoại không đúng, số điện thoại bàn thì sẽ không nhận được tin nhắn.

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

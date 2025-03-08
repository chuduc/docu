# Gửi tin Zalo quan tâm

Zalo quan tâm là dịch vụ gửi tin nhắn cho những khách hàng tương tác với Zalo OA của bạn.

{% hint style="info" %}
Gửi tin Zalo quan tâm chỉ có thể thực hiện được nếu bạn đang tương tác với khách hàng qua Zalo.

Bạn đã có tài khoản Zalo OA.

Khách hàng thực hiện trigger đã quan tâm Zalo OA của bạn.
{% endhint %}

Bạn phải chọn tài khoản Zalo OA cấu hình tại các Trigger đang có. Nếu chưa có tài khoản hãy tích hợp thêm, xem thêm tại [tich-hop-zalo.md](../../../tich-hop/huong-dan-tich-hop/tich-hop-zalo.md "mention").

1. Tìm và **chọn thêm hành động Gửi Tin Zalo quan tâm.**

<figure><img src="../../../.gitbook/assets/zalo quan tâm.png" alt=""><figcaption></figcaption></figure>

2. **Chọn loại tin nhắn gửi đi:**

* **Tin tư vấn**

Chỉ gửi được tin tư vấn nếu khách hàng có tương tác với OA trong vòng **7 ngày.**

Chỉ gửi được tin nhắn văn bản, hình ảnh, file đính kèm.

{% hint style="info" %}
Thời gian gửi tin Tư vấn 24/24
{% endhint %}

* **Tin giao dịch: thông báo cho khách hàng về giao dịch**

Chỉ gửi được tin giao dịch nếu khách hàng có tương tác với OA trong vòng 1 năm.

Zalo sẽ dựa vào tỉ lệ báo xấu của User với OA để đánh giá và có các hình thức xử lý đối với các trường hợp OA dùng tin Giao dịch sai mục đích, làm phiền người dùng, ...

Mẫu tin theo quy định của Zalo.

{% hint style="info" %}
Thời gian gửi tin giao dịch 24/24
{% endhint %}

* **Tin truyền thông**

Gửi được với tất cả các khách hàng đang quan tâm Zalo OA của bạn.

Số lượng tin truyền thông 1 khách hàng nhận trong 1 tháng áp dụng theo gói dịch vụ OA của bạn.

Số lượng tin truyền thông 1 khách hàng nhận trong 1 ngày là 1 tin.

3. **Điền nội dung tin nhắn** theo loại tin nhắn gửi đi.
4. **Thêm hành động bổ sung**: khi gửi tin thành công, khi gửi tin thất bại.
5. **Chọn tài khoản cấu hình Zalo,** nếu chưa có hãy tích hợp thêm xem thêm tại [tich-hop-zalo.md](../../../tich-hop/huong-dan-tich-hop/tich-hop-zalo.md "mention")

{% hint style="info" %}
Thời gian gửi tin Truyền thông Từ 6h00 -> 21h59
{% endhint %}

### Tạo tin tư vấn

1 tin tư vấn chỉ được chứa văn bản hoặc hình ảnh hoặc file.

1. **Tin nhắn văn bản**

Với các tin văn bản, bạn có thể thêm nút với các hành động khác nhau.

2. **Tin nhắn hình ảnh**

Với tin nhắn hình ảnh, bạn chỉ có thể upload ảnh jpg, png với dung lượng tối đa 1MB. Bạn cũng có thể nhập đường dẫn của ảnh tại đây.

<figure><img src="../../../.gitbook/assets/nhập đường dẫn ảnh.png" alt=""><figcaption></figcaption></figure>

3. **Tin nhắn File**

Bạn chọn file và tải lên, hệ thống chỉ cho phép tải file **PDF, DOC và DOCX** dung lượng tối đa **5MB**

### Tạo tin giao dịch

1. **Tải ảnh lên hoặc chèn URL:** **Tối đa 1MB**, chấp nhận loại file **.png, .jpg,** .**jpeg, .gif, .svg**
2. **Nhập tiêu đề tin nhắn**
3. **Nhập mô tả**
4.  **Điền thông tin giao dịch**

    *   **Thông tin khách hàng**\
        Nếu bạn  chọn Tên khách hàng, bạn hãy chọn trường thông tin lưu tên khách hàng của bạn\
        Nếu bạn chọn Mã khách hàng, bạn được tuỳ chỉnh thông tin hiển thị trên tin nhắn. Ví dụ bạn muốn hiển thị Mã đơn hàng và hiển thị thông tin mã đơn hàng bạn nhập như sau.\


        <figure><img src="../../../.gitbook/assets/mã đơn hàng.png" alt=""><figcaption></figcaption></figure>
    * **Loại tin nhắn**: bạn chọn loại tin nhắn mà Zalo cung cấp tuỳ theo mục đích sử dụng.
    * **Tin nhắn có trạng thái:** nếu bạn muốn hiển thị thông tin trạng thái trong tin nhắn của bạn. Ví dụ như hình sau:

    ![](../../../.gitbook/assets/Screenshot_2023-09-26-14-13-39-797_com.zing.zalo.jpg)

    * **Các trường thông tin khác**: Bạn có thể thêm các thông tin khác muốn hiển thị trên tin nhắn.
5. **Nhập mô tả**: nhập thông tin mô tả.
6. Thêm nút CTA nếu có.

{% hint style="info" %}
Xem màn hình preview để xây dựng nội dung tin nhắn phù hợp.
{% endhint %}

### Tạo tin truyền thông

1. **Tải ảnh lên hoặc chèn URL**: **Tối đa 1MB**, chấp nhận loại file **.png, .jpg,** .**jpeg, .gif, .svg**
2. **Nhập tiêu đề tin nhắn**:nhập tiêu đề tin nhắn.
3. **Nhập mô tả:** nhập thông tin mô tả.
4. **Nhập thông tin truyền thông** nếu muốn hiển thị các thông tin liên quan đến khách hàng.
5. **Nhập mô tả hiển thị phía dưới tin nhắn.**
6. Thêm nút CTA nếu có, và chọn hành động tương ứng.

Để cá nhân hóa nội dung tin nhắn theo từng khách hàng, xem thêm tại [ca-nhan-hoa-noi-dung-thong-diep-theo-tung-khach-hang.md](../../../meo-su-dung-ladiflow/ca-nhan-hoa-noi-dung-thong-diep-theo-tung-khach-hang.md "mention")

Để nối 2 hành động trong cùng 1 Flow bạn xem thêm tại đây [lam-sao-de-noi-2-hanh-dong-trong-flow.md](../lam-sao-de-noi-2-hanh-dong-trong-flow.md "mention")

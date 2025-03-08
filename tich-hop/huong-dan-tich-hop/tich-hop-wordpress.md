# Tích hợp Wordpress

Kể từ sau thời điểm tích hợp Wordpress trên LadiFlow thành công:

* Tất cả khách hàng mới tạo đều được đồng bộ sang LadiFlow
* Tất cả đơn hàng mới tạo, cập nhật, huỷ sẽ cập nhật dữ liệu khách hàng đã có hoặc tạo mới khách hàng
* Tự động cập nhật các thông tin chỉ số liên quan đến đơn hàng của bạn và của từng khách hàng

{% hint style="info" %}
**Lưu ý:**&#x56;ới các thông tin thời gian, LadiFlow nhận dữ liệu theo format: mm/dd/yyy ( tháng/ngày/năm). Nếu dữ liệu mà LadiFlow nhận được sai format sẽ dẫn tới sai hoặc lỗi dữ liệu.
{% endhint %}

### 1. **Cài đặt Plugin LadiPage trong Wordpress.**

1. Đăng nhập trang quản trị website WordPress của bạn với **quyền Admin.**
2. Tại menu **Plugins** chọn **Add New** để cài đặt plugins mới.
3. Chọn Tệp file plugin LadiPage để cài đặt plugin vào Wordpress. Tải file [TẠI ĐÂY](https://drive.google.com/file/d/1nu-atpCcIfyEFx4T5bAK-nCb9cKwr6dr/view)

<figure><img src="https://img001.prntscr.com/file/img001/ilQUPxjlQ-yXP1DzEVRWBQ.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Trong trường hợp tải file.ladipage báo lỗi, vui lòng kiểm tra lại thông tin hosting, xem cấp quyền tải file không.
{% endhint %}

4.  Bấm chọn app LadiApp vừa cài, sau đó sao chép lại nội dung trong 2 ô **API KEY** và **API URL (Lưu ý: bấm Save Changes sau khi lấy API).**\


    <figure><img src="../../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>

### 2. Tích hợp tài khoản Wordpress

1. Tìm và chọn ứng dụng **Wordpress** trên danh sách ứng dụng tích hợp.

<figure><img src="../../.gitbook/assets/image (415).png" alt=""><figcaption></figcaption></figure>

2. Chọn **Thêm liên kết**.
3. Mở 1 cửa sổ trình duyệt mới, truy cập vào trang Wordpress và đăng nhập với tài khoản của bạn.
4. Trên Wordpress, chọn **LadiApp**. **Copy API Key**, **Website URL** lần lượt paste vào **API Key và API URL trên Form lưu liên kết trên LadiFlow**. Chọn **Save changes trên wordpress** để lưu dữ liệu.

<figure><img src="../../.gitbook/assets/image (418).png" alt=""><figcaption></figcaption></figure>

5. **Đặt tên cho tích hợp** của bạn và chọn **Lưu liên kết**.

**Hiện tại hệ thống không giới hạn số tích hợp Wordpress.**

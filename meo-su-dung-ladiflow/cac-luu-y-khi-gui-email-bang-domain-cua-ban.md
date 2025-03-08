# Các lưu ý khi gửi Email bằng domain của bạn

Khi bạn sử dụng tên miền để gửi email trên LadiFlow bạn sẽ gặp nhiều vấn đề trong quá trình thiết lập trên LadiFlow. Bài viết này sẽ giúp bạn hiểu rõ hơn việc sử dụng gửi email bằng domain và các lưu ý khi sử dụng.

### Các bước để gửi Email bằng domain

1. Truy cập **Cài đặt -> Quản lý tên miền -> Thêm mới tên miền**
2. **Điền tên miền của bạn và chọn Thêm mới tên miền**
3. **Mở trang quản lý tên miền trong tab mới**
4. **Lần lượt tạo các bản ghi DNS yêu cầu LadiFlow trên tên miền của bạn**. Để xem hướng dẫn tạo bản ghi DNS xem thêm tại [cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien](../cach-tao-ban-ghi-theo-ten-mien-tren-cac-website-quan-ly-ten-mien/ "mention")

LadiFlow cung cấp 3 phương thức xác thực: DKIM, SPF, DMARC tương ứng với từng bản ghi:

**Bản ghi DKIM**\


<figure><img src="../.gitbook/assets/image (26).png" alt="" width="563"><figcaption></figcaption></figure>

**Bản ghi SPF**

<figure><img src="../.gitbook/assets/image (27).png" alt="" width="563"><figcaption></figcaption></figure>

**Bản ghi DMARC**

<figure><img src="../.gitbook/assets/image (28).png" alt="" width="563"><figcaption></figcaption></figure>

5. Sau khi tạo các bản ghi, **chờ ít nhất vài phút để các bản ghi áp dụng vào tên miền của bạn và chờ hệ thống kiểm tra trạng thái Tracking SSL**.&#x20;
6. Sau khi Trạng thái Tracking SSL đã được bật, bấm nút **Xác thực** để hệ thống tiến hành xác thực bản ghi.

<figure><img src="../.gitbook/assets/image (29).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
Trạng thái tên miền chuyển sang **Đã xác thực,** bạn có thể bắt đầu sử dụng email theo tên miền để thêm liên kết tích hợp email, xem thêm tại [tich-hop-email.md](../tich-hop/huong-dan-tich-hop/tich-hop-email.md "mention").
{% endhint %}

{% hint style="info" %}
**Lưu ý**: Trạng thái xác thực trên LadiFlow là trạng thái xác thực DKIM, để kiểm tra các phương thức khác xem hướng dẫn tại [#chu-dong-kiem-tra-xac-thuc-danh-tinh-dkim-spf-dmarc](cac-luu-y-khi-gui-email-bang-domain-cua-ban.md#chu-dong-kiem-tra-xac-thuc-danh-tinh-dkim-spf-dmarc "mention")
{% endhint %}

### Xác thực không thành công thì phải làm sao?

* LadiFlow hiện tại đang kiểm tra xác thực qua các bản ghi DKIM, nếu chưa xác thực thành công bạn cần kiểm tra lại các bản ghi DNS DKIM trên tên miền xem đã đúng và đủ như LadiFlow yêu cầu chưa.
* Sử dụng các công cụ kiểm tra DNS để kiểm tra xem các bạn ghi bạn tạo trên trang quản lý tên miền đã áp dụng chưa. Ví dụ: [https://dnschecker.org/](https://dnschecker.org/) Các bản ghi cần thời gian để có thể áp dụng, tối đa 24h.
* Nếu bạn đã thêm sai bản ghi, cần xóa đi và thêm lại bản ghi mới vì thường thời gian để cập nhật bản ghi sẽ lâu hơn tạo mới bản ghi.
* Kiểm tra lại các bản ghi đã có trên tên miền với các bản ghi của LadiFlow xem có mâu thuẫn gì không.

### Lưu ý khi xác thực DKIM

1. Một số trang quản lý tên miền cho phép bạn xác thực DKIM cho tên miền, và có thể các bản ghi của trang quản lý tên miền đó mâu thuẫn với LadiFlow dẫn tới bạn không thể gửi thư hoặc xác thực không thành công. Vậy trong trường hợp này, bạn cần làm gì:

* Ưu tiên các bản ghi xác thực DKIM của LadiFlow. Vì bạn sừ dụng LadiFlow để gửi thư, do đó bạn cần xác thực DKIM trên LadiFlow để đảm bảo thư có thể gửi được.
* Việc xác thực DKIM trên trang quản lý tên miền là không bắt buộc, nếu có thể xác thực cả 2 mà không gặp vấn đề gì thì bạn có thể giữ tất cả bản ghi của trang quản lý tên miền gợi ý.

2. Nếu bạn đăng ký dịch vụ mail server:  gmail, yoho, outlook... Các nền tảng này sẽ yêu cầu bạn cần xác thực DKIM thì bạn phải:

* Xác thực DKIM của cả mail server và LadiFlow yêu cầu bằng cách tạo lần lượt các bản ghi&#x20;
  * Xác thực DKIM của mail server
  * Xác thực DKIM của LadiFlow
* Nếu gặp vấn đề về bản ghi, hãy cố gắng thử loại bản ghi DNS khác (nếu mail server cho phép).
* Nếu không thể giải quyết, hãy liên hệ với CSKH bằng live chat để được hỗ trợ.

### Lưu ý khi xác thực SPF

Một tên miền chỉ được tồn tại một bản ghi xác thực SPF, do đó nếu tên miền bạn đang sở hữu có từ 2 bản ghi xác thực SPF ( loại là TXT, có value v=spf1) thì bạn thực hiện gộp 2 bản ghi thành 1, và xóa bản ghi còn lại theo công thức như sau:

* Type: TXT
* Host: \<tên miền của bạn>
* Value: v=spf1 \<ip> \<danh sách server> \~all

Ví dụ bạn tồn tại 2 bản ghi sau

Bản ghi 1: TXT v=spf1 ip4:197.168.25.25 \~all

Bản ghi 2: TXT v=spf1 include:\_spf.google.com include:amazonses.com \~all

Bản ghi gộp: TXT v=spf1  ip4:197.168.25.25 include:\_spf.google.com include:amazonses.com \~all

Nếu bạn sử dụng dịch vụ email server: gmail, outlook, yoho thì bạn cần chọn đúng nền tảng gửi và nhận mail, sau đó tạo bản ghi DNS tương ứng.

### Chủ động kiểm tra xác thực danh tính DKIM, SPF, DMARC

Trạng thái xác thực trên LadiFlow là trạng thái xác thực DKIM, để kiểm tra trạng thái xác thực DKIM, SPF và DMARC bạn thực hiện gửi một email tới tài khoản email của bạn và làm như sau:

1. Mở hòm thư, tìm đúng email bạn vừa gửi bằng tên miền.
2. Chọn Hiển thị thư gốc

<figure><img src="../.gitbook/assets/image (251).png" alt="" width="429"><figcaption></figcaption></figure>

3. Kiểm tra trạng thái xác thực SPF, DKIM, DMARC:

<figure><img src="../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

Trạng thái PASS: đã xác thực thành công

Trạng thái FAIL: xác thực thất bại.

Bạn cần kiểm tra các bạn ghi để đảm bảo cả 3 phương thức xác thực, email của bạn đều xác thực thành công.

### Nếu muốn quản lý gửi và nhận thư từ email theo domain thì phải làm gì?

Để quản lý email đã gửi và nhận từ email domain bạn cần đăng ký dịch vụ email server : Gmail, Outlook... Khi đó bạn cần phải thực hiện các bước xác thực mà các mail server này yêu cầu. Việc đăng ký dịch vụ mail server giúp bạn có thể nhận các phản hồi của khách hàng qua thư. Dịch vụ này sẽ mất thêm một khoản phí tùy theo từng nhà cung cấp.

Nếu không đăng ký dịch vụ mail server, bạn chỉ có thể gửi thư trên LadiFlow, bất kỳ phản hồi của khách hàng với thư của bạn, bạn sẽ không thể nhận và xem chúng. Các loại email này thường phù hợp với email thông báo, không nhận phản hồi.

{% hint style="info" %}
Trạng thái tên miền chuyển sang **Đã xác thực,** bạn có thể bắt đầu sử dụng email theo tên miền để thêm liên kết tích hợp email, xem thêm tại [tich-hop-email.md](../tich-hop/huong-dan-tich-hop/tich-hop-email.md "mention").
{% endhint %}

### Bổ sung bản ghi TRACKING theo tên miền

Ngoài các bản ghi xác thực tên miền theo 3 phương thức ở trên, LadiFlow còn cung cấp bản ghi Tracking nhằm:&#x20;

* Theo dõi lượt mở và lượt click link trong các chiến dịch, kịch bản gửi email
* Giảm nguy cơ email bị đánh dấu là spam.&#x20;

Bạn cần tạo bản ghi Tracking theo hướng dẫn tại [Quản lý tên miền](../cai-dat/cai-dat-chung/quan-ly-ten-mien.md#ban-ghi-tracking).

<figure><img src="../.gitbook/assets/image (30).png" alt="" width="563"><figcaption></figcaption></figure>

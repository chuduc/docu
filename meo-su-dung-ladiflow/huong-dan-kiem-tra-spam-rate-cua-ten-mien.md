# Hướng dẫn kiểm tra Spam rate của tên miền

Công cụ Postmaster của Google cho phép người gửi Email có thể theo dõi các số liệu chính về khả năng gửi thư: báo cáo spam của người dùng, danh tiếng tên miền Gmail.  Dưới đây là hướng dẫn thiết lập công cụ Postmaster và hướng dẫn xem dữ liệu trên công cụ này.

### Hướng dẫn thiết lập công cụ Postmaster của Google

{% hint style="info" %}
Bạn cần có tài khoản google ( Tài khoản gmail hoặc Workspace) để sử dụng công cụ Postmaster. Nếu bạn chưa có, hãy tạo 1 tài khoản google.&#x20;
{% endhint %}

1. Đăng nhập vào trang [https://postmaster.google.com](https://postmaster.google.com/).&#x20;
2. Chọn nút + dưới đây để thêm tiên miền

<figure><img src="../.gitbook/assets/image (196).png" alt="" width="563"><figcaption></figcaption></figure>

3. Điền tên miền gốc của bạn vào ô dưới đây, sau đó chọn **Following**\
   **Lưu ý: không nhập subdomain, hãy nhập tên miền gốc.**

<figure><img src="../.gitbook/assets/image (199).png" alt="" width="484"><figcaption></figcaption></figure>

4. Thêm bản ghi TXT theo hướng dẫn của Postmaster vào tên miền của bạn

<figure><img src="../.gitbook/assets/image (200).png" alt="" width="482"><figcaption></figcaption></figure>

Nếu bạn không thể thêm bản ghi TXT, bạn có thể đổi sang bản ghi CNAME bằng cách chọn vào a CNAME record như hình dưới đây

<figure><img src="../.gitbook/assets/image (201).png" alt="" width="482"><figcaption></figcaption></figure>

Thông tin bản ghi CNAME sẽ hiển thị, bạn tạo bản ghi với các thông tin yêu cầu

<figure><img src="../.gitbook/assets/image (202).png" alt="" width="491"><figcaption></figcaption></figure>

Sau khi tạo bản ghi TXT hoặc CNAME, bạn chọn **TO VALIDATE** để công cụ kết nối với tên miền của bạn

Nếu kết nối thành công, tên miền của bạn sẽ được đổi sang trạng thái Valid

<figure><img src="../.gitbook/assets/image (204).png" alt="" width="563"><figcaption></figcaption></figure>

Nếu kết nối thất bại, bạn cần kiểm tra nội dung bản ghi DNS bạn vừa thêm

<figure><img src="../.gitbook/assets/image (203).png" alt="" width="479"><figcaption></figcaption></figure>

### Hướng dẫn xem dữ liệu trên công cụ Postmaster

Google sẽ tổng hợp dữ liệu hàng ngày, nghĩa là sau khi bạn gửi thư, cần 24 giờ để dữ liệu được tổng hợp báo cáo. Nếu bạn gửi với số lượng ít, thông tin sẽ cập nhật lâu hơn và có thể sẽ không thể hiển thị dữ liệu. Thông thường, bạn cần gửi thư cho 100-200 email khác nhau để Google có thể tổng hợp dữ liệu tổng quan cho bạn.

Mặc định dữ liệu sẽ hiển thị dựa trên lượng gửi tin 7 ngày gần đây. Nếu không có dữ liệu, bạn có thể xem dữ liệu cách dây 120 ngày để có dữ liệu từ các tháng trước.

Để xem dữ liệu tại tên miền nào, bạn chọn vào tên miền đó( tên miền đã được xác thực trên Postmaster)

Chọn xem các chỉ số báo cáo tại đây

<figure><img src="../.gitbook/assets/image (209).png" alt="" width="563"><figcaption></figcaption></figure>

#### Chỉ số SPAM Rate

Bạn có thể xem được tỷ lệ người nhận thư báo cáo thư của bạn là spam so với số thư vào inbox. Lưu ý rằng, theo Google nếu thư của bạn bị gửi thẳng vào hộp thư Spam thì tỷ lệ spam rate sẽ thấp một cách lạ thường.

> “If a substantial number of emails are delivered directly to spam folders, you may see a low spam rate even though users may still be marking your inboxed emails as spam.”

<figure><img src="../.gitbook/assets/image (205).png" alt="" width="563"><figcaption></figcaption></figure>

#### Theo dõi danh tiếng tên miền

Danh tiếng người gửi đóng vai trò quan trọng trong việc gửi thư. Nếu danh tiếng người gửi cao đồng nghĩa với việc tỷ lệ thư vào inbox cao hơn tỷ lệ vào spam.

<figure><img src="../.gitbook/assets/image (206).png" alt="" width="563"><figcaption></figcaption></figure>

Gmail phân cấp danh tiếng tên miền theo 4 cấp độ

* **High**: tên miền của bạn có thành tích tỷ lệ thư vào hộp thư spam thấp và tuân thủ theo các nguyên tắc dành cho người gửi của Gmail. Thư hiếm khi bị bộ lọc spam đánh dấu.
* **Medium**: Chất lượng gửi thư tốt, lượng thư rác thấp. Hầu hết thư được gửi vào inbox trừ một số trường hợp mức độ thư rác tăng đáng kể.
* **Low**: Thường xuyên gửi một lượng thư rác cao. Thư được gửi từ tên miền này có thể bị đánh dấu là thư rác.
* **Bad**: Lượng thư rác quá cao. Hầu hết số thư được gửi từ tên miền này bị đánh dấu là Spam hoặc bị bộ lọc Spam đánh dấu.

#### Xác thực nội dung

Chỉ số này cho phép bạn xem tỷ lệ email xác thực bởi các giao thức DKIM, SPF và DMARC.&#x20;

Có 3 chỉ số trên biểu đồ:

* Tỷ lệ SPF thành công: Tỷ lệ thư xác thực SPF trên tổng số thư được gửi từ tên miền( bao gồm cả các thư giả mạo).
* Tỷ lệ DKIM thành công: Tỷ lệ thư xác thực DKIM trên tổng số thư được gửi từ tên miền( bao gồm cả các thư giả mạo).
* Tỷ lệ DMARC thành công: Tỷ lệ thư xác thực DMARC trên tổng số thư được gửi từ tên miền( bao gồm cả các thư giả mạo).

<figure><img src="../.gitbook/assets/image (208).png" alt="" width="563"><figcaption></figcaption></figure>

Ngoài ra, trên cộng cụ Postmaster còn có rất nhiều các báo cáo khác, bạn có thể tham khảo thêm [TẠI ĐÂY](https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/google-postmaster)

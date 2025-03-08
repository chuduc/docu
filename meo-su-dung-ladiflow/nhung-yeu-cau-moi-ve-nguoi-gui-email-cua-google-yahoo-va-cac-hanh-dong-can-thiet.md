# Những yêu cầu mới về người gửi Email của Google, Yahoo và các hành động cần thiết

Google và Yahoo đã có thông báo về những sự thay đổi về các yêu cầu của người gửi Email. Những sự thay đổi này sẽ bắt đầu áp dụng từ 01/02/2024.&#x20;

### Những yêu cầu mới về người gửi Email của Google và Yahoo

Bắt đầu từ 01/02/2024, Google và Yahoo đưa ra các yêu cầu về người gửi Email với **tập khách hàng nhận tin có địa chỉ email của Gmail, Googlemail, hoặc địa chỉ Google Workspace .** Tất cả các email gửi bằng tên miền phải được xác thực để tránh giả mạo trong email gửi tin và tên người gửi.

Những yêu cầu mới này nhằm mục đích bảo vệ người dùng khỏi những thư rác. Những người nhận được thư thực sự họ mong muốn nhận được thư từ bạn. Do đó danh tiếng người gửi, tỷ lệ báo xấu là một trong những yếu tố để đo lường. Bạn có thể xem đầy đủ các yêu cầu trong [Trung tâp trợ giúp Gmai](https://support.google.com/a/answer/81126?visit_id=638410716736986358-1672109054\&rd=1)[l](https://support.google.com/a/answer/81126?visit_id=638410716736986358-1672109054\&rd=1).

Nếu bạn mong muốn thư của bạn vào hòm thư người gửi, bạn phải tuân thủ theo các yêu cầu về xác thực người gửi và ngăn chặn spam. Để làm được điều này bạn cần:

#### **Yêu cầu với tất cả tài khoản gửi thư**

1. **Không sử dụng địa chỉ email cá nhân để gửi thư ( @gmail, @googlemail, @outlook,...).**
2. **Xác thực danh tính người gửi bằng DKIM, SPF.**\
   [**Xem hướng dẫn tại đây.**](cac-cach-xac-thuc-danh-tinh-nguoi-gui-email.md)
3. **Giảm tỷ lệ email trả về( Complaint rate) và duy trì dưới 0.3%.**\
   Giữ tỷ lệ spam rate duy trì dưới 0,3% tại [Postmaster tool](https://gmail.com/postmaster/) của Gmail. Nếu bạn chưa có tài khoản hãy đăng ký.\
   Nếu tỷ lệ spam rate đạt 0,3%, bạn cần xem xét lại nội dung email, đọc các bài viết sau:\
   [Vấn đề gặp phải khi gửi Email](cac-van-de-gap-phai-khi-gui-email.md), [Kiểm tra tỷ lệ vào inbox, spam](kiem-tra-ty-le-vao-inbox-spam.md)\
   Nếu bạn đạt tỷ lệ spam rate lớn hơn 0.3%, tỷ lệ thư của bạn vào hòm thư của người nhận rất thấp.

#### **Yêu cầu với tài khoản gửi thư trên 5.000 thư/ngày với 1 địa chỉ gửi thư**

1. **Thiết lập DMARC cho tên miền**.\
   Team LadiFlow đang tích cực làm việc và sẽ hoàn thiện tính năng này trước ngày 01/02/2024.
2. **Thiết lập địa chỉ người gửi tuân thủ tương ứng với tên miền theo quy chuẩn của DMARC.**\
   Tên người gửi cần tương thích với tên miền theo quy chuẩn của DMARC. Ví dụ tên miền của bạn là ladipage.vn, thì Email gửi thư hợp lệ là sale@ladipage.vn, support@ladipage.vn
3. **Hủy đăng ký bằng click vào 1 link ( one-click unsubscribe)**\
   Team LadiFlow đang tích cực làm việc và sẽ hoàn thiện tính năng này trước ngày 01/02/2024. Tất cả các email gửi từ LadiFlow sẽ tự động đáp ứng yêu cầu này.

{% hint style="info" %}
Lưu ý, số lượng thư gửi theo ngày được tính theo tên miền gốc. Ví dụ bạn gửi từ địa chỉ sale@ladipage.vn 300 thư, support@ladipage.vn 500 thư thì Google sẽ tính tên miền ladipage.vn là 800 thư.
{% endhint %}

{% hint style="info" %}
Chỉ cần bạn xác thực thành công tên miền trên LadiFlow bằng DKIM và SPF, bạn có thể sử dụng email theo tên miền đó để gửi tin mà không cần phải đăng ký dịch vụ Email.

Nếu bạn đăng ký dịch vụ Email, bạn có thể nhận, đọc các email phản hồi(reply) từ khách hàng của bạn.
{% endhint %}

### LadiFlow sẽ có những thay đổi gì vào ngày 01/02/2024?

1. **Không cho phép sử dụng email cá nhân khi thêm liên kết tích hợp email.**
2. **Tạm dừng tất cả Campaign, Sequence, Flow đã cấu hình tích hợp gửi bằng email cá nhân vào 23:00 ngày 31/01/2024** . Bạn cần phải thay đổi các tài khoản email cá nhân sang Email theo tên miền riêng và cập nhật lại thiết lập tài khoản trên các Campaign, Sequence, Flow để đảm bảo các kịch bản hoạt động.
3. **Bổ sung tính năng thiết lập DMARC cho tên miền.**
4. **Bổ sung tính năng one-click unsubcribe áp dụng toàn bộ Email gửi từ LadiFlow.**

## FAQ

### Những ai sẽ bị ảnh hưởng bởi những yêu cầu này?

**Tất cả tài khoản sử dụng Email để tương tác với khách hàng, đặc biệt với những khách hàng gửi nhiều hơn 5000 email/ngày.** Việc tuân thủ các chỉnh sách của Google và Yahoo giúp nâng cao tỷ lệ vào inbox, giảm tỷ lệ Spam.

### Nếu không đáp ứng những yêu cầu này thì sẽ như thế nào?

Nếu bạn không đáp ứng những yêu cầu về người gửi của Google và Yahoo, **tin của bạn sẽ không được gửi hoặc bị rơi vào hộp thư spam.**&#x20;

Với LadiFlow, chúng tôi sẽ ngừng cho phép gửi mail sử dụng email cá nhân và bổ sung thêm các tính năng để đáp ứng yêu cầu của Google và Yahoo.

### Tôi có tên miền nhưng không sử dụng dịch vụ Email nào thì có gửi được Email trên LadiFlow không?

Có. Bạn hoàn toàn có thể gửi được Email trên LadiFlow khi tên miền đã được xác thực mà không cần sử dụng dịch vụ Email nào khác như Gmail for Business, Outlook, Zoho,… với nhu cầu chỉ gửi Email. Trường hợp bạn cần gửi và nhận thì bạn cần sử dụng 1 trong các nền tảng email như Gmail for Business, Outlook, Zoho với tên miền này và vẫn gửi được Email với LadiFlow

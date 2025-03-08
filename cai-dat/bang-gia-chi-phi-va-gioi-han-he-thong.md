# Bảng giá chi phí và giới hạn hệ thống

### Bảng giá chi phí&#x20;

#### **Từ ngày 01.04.2024**

Từ ngày 01.04.2024, LadiFlow sẽ thay đổi cơ chế tính phí giao dịch từ đơn vị API Credit sang đơn vị Điểm.&#x20;

Với số dư API credit đang có trên tài khoản của bạn, chúng tôi sẽ quy đổi sang đơn vị Điểm theo công thức sau:

```
Số dư điểm = Số dư API credit x 100
```

<table><thead><tr><th width="243.33333333333331">Tính năng</th><th width="233">Chi phí</th><th>Ghi chú</th></tr></thead><tbody><tr><td>Gửi Email</td><td>2 Điểm/tin</td><td></td></tr><tr><td>Zalo quan tâm: tin tư vấn </td><td>1000 tin nhắn miễn phí/tháng<br>8 tin tư vấn miễn phí<br>55 vnđ/tin với các tin tính phí<br>1 Điểm/ tin nhắn</td><td><br>Sau khi khách hàng tương tác lại sau 48h số lượng tin tư vấn miễn phí reset 8 tin với khách hàng đó.<br>Nếu khách hàng không tương tác sau 48h sẽ trừ từ tổng số tin nhắn miễn phí đang còn, sau đó tính phí các tin tiếp theo.</td></tr><tr><td>Zalo quan tâm: tin giao dịch</td><td>165 vnđ/tin<br>1 Điểm/ tin nhắn</td><td></td></tr><tr><td>Zalo quan tâm: tin truyền thông</td><td>1 Điểm/tin nhắn</td><td></td></tr><tr><td>Zalo ZNS</td><td>200-1500vnđ/tin<br>1 Điểm/tin nhắn</td><td></td></tr><tr><td>Đồng bộ dữ liệu với bên thứ 3 (Zoom, Google Sheet,...)</td><td>1 Điểm/ lượt chạy</td><td></td></tr><tr><td>HTTP Request</td><td>1 Điểm/ lượt chạy</td><td></td></tr><tr><td>SMS</td><td>1 Điểm/tin</td><td>Chi phí của nhà mạng từ 400-800 vnđ/tin và thanh toán trực tiếp với ESMS</td></tr><tr><td>AI Call</td><td>1 Điểm/lượt gọi<br>Chi phí=số block x đơn giá 1 block</td><td>30 giây tính 1 block. Thời gian tính block từ lúc khách hàng nhận cuộc gọi đến khi tắt máy<br>Đơn giá của 1 block tùy vào loại cuộc gọi, cụ thể:<br>- Cố định: 600 vnđ/block<br>- Cá nhân hóa: 694 vnđ/block<br>- Voice OTP: 300 vnđ/block</td></tr><tr><td>Messenger</td><td>1 điểm/hành động<br>1 điểm/tin nhắn</td><td>Hành động gồm có: like, trả lời bình luận<br>Tin nhắn: tính riêng theo từng nội dung.</td></tr><tr><td>Email AI, Nội dung AI</td><td><p>Gọi T=Tổng số token/1000</p><p>       X: phần nguyên của T</p><p>       Z: phần thập phân của T</p><p><span class="math">Số Điểm = \begin{cases}    3*X+2 &#x26;\text{if } Z \le 0.5\\    3*(X+1)  &#x26;\text{if } Z \gt 0.5  \end{cases}</span></p></td><td>Giá trị Tổng số token do OpenAI trả về</td></tr><tr><td>Các hành động khác</td><td>1 Điểm/lượt chạy</td><td><ul><li>Thêm Tag</li><li> Xóa Tag </li><li>Thêm trường tùy chỉnh</li><li>Xóa trường tùy chỉnh </li><li>Đăng kí Sequence </li><li>Hủy đăng ký theo dõi Sequence </li><li>Điều chỉnh Lead Scoring</li><li>Phân phối Voucher</li><li>Bắt đầu một Flow khác </li><li>Điều kiện</li><li>Hẹn giờ </li><li>Push Notification (Web)</li><li>Gửi tin LadiChat</li><li>Gửi thông báo telegram</li><li>Thêm thành viên vào cuộc họp, webinar Zoom</li><li>Tiktok ads postback</li><li>Thêm khách hàng vào sự kiện google calendar</li></ul></td></tr></tbody></table>

#### **Trước ngày 01.04.2024**

<table><thead><tr><th width="229.33333333333331">Tính năng</th><th width="278">Chi phí (trước 01.04.2024)</th><th>Ghi chú</th></tr></thead><tbody><tr><td>Gửi Email</td><td>0.03 credit/tin</td><td></td></tr><tr><td>Zalo quan tâm: tin tư vấn </td><td>1000 tin nhắn miễn phí/tháng<br>8 tin tư vấn miễn phí<br>55 vnđ/tin với các tin tính phí<br>0.01 credit/ tin nhắn</td><td><br>Sau khi khách hàng tương tác lại sau 48h số lượng tin tư vấn miễn phí reset 8 tin với khách hàng đó.<br>Nếu khách hàng không tương tác sau 48h sẽ trừ từ tổng số tin nhắn miễn phí đang còn, sau đó tính phí các tin tiếp theo.</td></tr><tr><td>Zalo quan tâm: tin giao dịch</td><td>165 vnđ/tin<br>0.01 credit/ tin nhắn</td><td></td></tr><tr><td>Zalo quan tâm: tin truyền thông</td><td>0.01 credit/ tin nhắn</td><td></td></tr><tr><td>Zalo ZNS</td><td>200-1500vnđ/tin<br>0.01 credit/tin nhắn</td><td></td></tr><tr><td>Đồng bộ dữ liệu với bên thứ 3 (Zoom, Google Sheet,...)</td><td>0.01 credit/lượt chạy</td><td></td></tr><tr><td>HTTP Request</td><td>0.01 credit/lượt chạy</td><td></td></tr><tr><td>SMS</td><td>0.01 credit/tin</td><td>Chi phí của nhà mạng từ 400-800 vnđ/tin và thanh toán trực tiếp với ESMS</td></tr><tr><td>AI Call</td><td>0.01 credit+ số block x 600 vnđ</td><td>30 giây tính 1 block. Thời gian tính block từ lúc khách hàng nhận cuộc gọi đến khi tắt máy</td></tr><tr><td>Messenger</td><td><p>0.01 credit/hành động </p><p>0.01 credit/tin nhắn</p></td><td>Hành động gồm có: like, trả lời bình luận<br>Tin nhắn: tính riêng theo từng nội dung.</td></tr><tr><td>Email AI, Nội dung AI</td><td><p>Gọi T=Tổng số token/1000</p><p>       X: phần nguyên của T</p><p>       Z: phần thập phân của T</p><p><span class="math">Số Credit = \begin{cases}    0.03*X+0.02 &#x26;\text{if } Z \le 0.5\\    0.03*(X+1)  &#x26;\text{if } Z \gt 0.5  \end{cases}</span></p></td><td>Giá trị Tổng số token do OpenAI trả về</td></tr><tr><td>Các hành động khác</td><td>0.01 credit/lượt chạy</td><td><ul><li>Thêm Tag</li><li> Xóa Tag </li><li>Thêm trường tùy chỉnh</li><li>Xóa trường tùy chỉnh </li><li>Đăng kí Sequence </li><li>Hủy đăng ký theo dõi Sequence </li><li>Điều chỉnh Lead Scoring</li><li>Phân phối Voucher</li><li>Bắt đầu một Flow khác </li><li>Điều kiện</li><li>Hẹn giờ </li><li>Push Notification (Web)</li><li>Gửi tin LadiChat</li><li>Gửi thông báo telegram</li><li>Thêm thành viên vào cuộc họp, webinar Zoom</li><li>Tiktok ads postback</li><li>Thêm khách hàng vào sự kiện google calendar</li></ul></td></tr></tbody></table>

### Giới hạn hệ thống

1. Trong khoảng thời gian **60** giây, 1 khách hàng chỉ được chạy flow 1 lần duy nhất, sau đó phải chờ để chạy lần tiếp theo. Nếu không, Flow sẽ không bị chặn không thể thực hiện được.
2. Với 1 flow, 1 khách hàng chỉ được chạy flow đó tối đa 20 lần/ngày. Sau đó Flow sẽ không thực hiện với khách hàng đó nếu tiếp tục kích hoạt trigger.&#x20;
3. Số lượng lượt chạy Flow, Campaign, Sequence trong ngày: Số lượt chạy Flow, số lượng tin gửi ở Campaign, Số lượng tin đã gửi ở Sequence được tính dựa theo số lượng khách hàng bạn có trên LadiFlow.

Nếu số lượng khách hàng của bạn <**6667**, số lượt chạy Trigger, Sequence của bạn là **20.000/ngày.**

Nếu số lượng khách hàng của bạn <**1667**, số lượng tin gửi Campaign của bạn là **5000**/**ngày**.

Nếu không, tính theo công thức sau:

* **Số lượng lượt chạy Trigger= số lượng khách hàng x3/ngày.**
* **Số lượng tin gửi Campaign= số lượng khách hàng x3/ngày.**
* **Số lượng tin gửi Sequence= số lượng khách hàng x3/ngày.**

Các tin nhắn hay lượt chạy Trigger vượt quá số lượng cho phép đều không thực hiện được.

**Lưu ý**:

* Số lượt lượt chạy/tin gửi sẽ tính trên số lượng gửi (không tính trên số lượng thành công/ đã nhận).
* Trường hợp khách hàng nhập thêm khách hàng thì số lượng này cũng sẽ tăng theo sau khi khách hàng được thêm mới.
* Tạm thời chưa giới hạn các request webhook của khách hàng.
* Sau **2h** sáng hàng ngày sẽ reset lại giới hạn request.

### Giới hạn số email gửi&#x20;

Số email gửi trong 1 ngày khác nhau theo từng tài khoản gmail bạn tích hợp. Con số này do Google quy định với mỗi người nhận email được tính là 1 tin và giới hạn sẽ được cập nhật sau 24h hàng ngày. Dưới đây là các số liệu mới nhất:&#x20;

| Loại giới hạn                                         | Giới hạn gửi                                                                       |
| ----------------------------------------------------- | ---------------------------------------------------------------------------------- |
| Số lượng email gửi/tài khoản                          | <ul><li>Google workspace: 2000/ngày</li><li>Tài khoản dùng thử: 500/ngày</li></ul> |
| Số người nhận/ tin khi gửi tin qua SMT hoặc Gmail API | <ul><li>100 </li></ul>                                                             |
| Số người nhận/tin trong Google Workspace              | Tối đa 2000 người/tin                                                              |

Nếu bạn gửi vượt quá giới hạn này trong ngày, các tin sau đó sẽ gửi thất bại.

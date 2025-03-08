# Cấu hình các giá trị mặc định khi sử dụng trường tùy chỉnh trong tin nhắn

Khi bạn sử dụng các trường tùy chỉnh khi cá nhân hóa thông điệp theo từng khách hàng, bạn sẽ gặp trường hợp mong muốn cài đặt trong thông điệp các giá trị mặc định hoặc  giá trị theo thời gian khách hàng vào kịch bản.&#x20;

### Đặt giá trị mặc định của trường tùy chỉnh

Khi bạn mong muốn cài giá trị mặc định cho một trường tùy chỉnh trong một thông điệp ( zalo, messenger, sms ...) trong trường hợp khách hàng không có dữ liệu trường tùy chỉnh này, bạn viết theo cấu trúc sau:

<pre><code><strong>{{tên trường mặc định|giá trị mặc định}}
</strong></code></pre>

Ví dụ:

```
{{full_name|Quý khách}}
{{thoi_gian_giao_hang|01/01/2024}}
```

Khi sử dụng thực tế sẽ như sau:

<figure><img src="../.gitbook/assets/image (627).png" alt="" width="468"><figcaption></figcaption></figure>

### Format các giá trị thời gian tùy ý

Để format các giá trị trường tùy chỉnh có kiểu dữ liệu là Ngày tháng tùy theo nhu cầu, LadiFlow cung cấp cho bạn cách viêt như sau:

```
{{<tên trường mặc định>|format(<định dạng>, <giá trị mặc định (optional)>)}}
```

Các định dạng hỗ trợ:

* yyyy/mm/dd HH:MM
* yyyy/mm/dd
* dd/mm/yyyy
* HH:MM dd/mm/yyyy
* HH:MM mm/dd/yyyy
* dd/mm/yyyy HH:MM

Lưu ý: giá trị mặc định là thông tin không bắt buộc.

Ví dụ:

```
{{created_at|format(yyyy/mm/dd HH:MM, 2022/04/03 14:00)}}
{{created_at|format(yyyy/mm/dd HH:MM, 2022/04/03 14:00)}}
{{created_at|format(yyyy/mm/dd HH:MM)}}
{{created_at|format(dd/mm/yyyy HH:MM)}}
{{created_at|format(HH:MM dd/mm/yyyy)}}
```

### Đặt các giá trị theo thời gian diễn ra

Nếu bạn muốn cài đặt các giá trị thời gian tương ứng với thời gian gửi tin, LadiFlow cũng cấp các mã thời gian tương ứng với từng nhu cầu khác nhau.

Nếu bạn sử dụng Campaign, thời gian theo thiết lập sau là thời gian gửi Campaign.

Nếu bạn sử dụng Sequence, Flow, thời gian theo thiết lập sau là thời gian gửi tin nhắn.

```
{{mã thời gian}}
Ví dụ: {{today}} => dd/mm/yyyy
```

**Danh sách các mã thời gian**&#x20;

| Mã thời gian           | Mô tả                                                                       |
| ---------------------- | --------------------------------------------------------------------------- |
| today                  | Thời điểm gửi tin                                                           |
| current\_day\_of\_week | <p>Thứ trong tuần tại thời điểm gửi tin<br>Ví dụ: Thứ Hai, Thứ Ba, ....</p> |
| current\_year          | <p>Năm của thời điểm gửi tin<br>Ví dụ: 2023, 2024...</p>                    |
| month                  | <p>Tháng của thời điểm gửi tin<br>Ví dụ: 1, 2, 3, 4, .. 11, 12</p>          |

{% hint style="info" %}
Với mã thời gian today, bạn có thể áp dụng quy tắc format giá trị thời gian. Xem các format [Tại  Đây](cau-hinh-cac-gia-tri-mac-dinh-khi-su-dung-truong-tuy-chinh-trong-tin-nhan.md#format-cac-gia-tri-thoi-gian-tuy-y).
{% endhint %}

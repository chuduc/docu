---
description: Sự kiện 1 Sequence đã hoàn thành với 1 khách hàng
---

# Hoàn tất 1 sequence

Khi khách hàng hoàn thành xong 1 Sequence đã cài đặt cho khách hàng đó, Trigger sẽ hoạt động. Nghĩa là tin nhắn cuối cùng được xuất bản trong Sequence đã được gửi cho khách.

1. Chọn **+Thêm Trigger**, chọn **Khi hoàn tất 1 Sequence** như hình dưới đây.

<figure><img src="https://lh5.googleusercontent.com/zW0BgFAXbZ0sqMVGYZquNzF3XS1BZdnnWR887Qz00FKSqj5YPBvHcqomg2uG5gV508mimhnU2Q3BQDG4ZDng231dUFvPQkAWbh8uEvAzCpteAzv3L85KBqac7dKuTZHdT1xPH2-GBxGdOkvyXazI47Y" alt=""><figcaption></figcaption></figure>

2. Điền các thông tin Điều kiện kích hoạt nếu muốn giới hạn tập khách hàng trong flow. Xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
3.  **Chọn sequence.** Nếu chưa có sequence nào bạn có thể thêm mới, xem thêm tại[Broken link](broken-reference "mention")\


    <figure><img src="../../../.gitbook/assets/image (689).png" alt="" width="473"><figcaption></figcaption></figure>

{% hint style="info" %}
1 khách hàng được tính là hoàn tất sequence khi họ được gửi tin kích hoạt cuối cùng trong chuỗi.

Nếu hệ thống đã đánh dấu khách hàng hoàn tất sequence, và bạn thao tác thêm tin vào chuỗi thì tin mới sẽ không được gửi khách hàng này.
{% endhint %}

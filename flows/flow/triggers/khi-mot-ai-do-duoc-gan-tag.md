---
description: Sự kiện khi gắn tag cho khách hàng
---

# Khi một ai đó được Gắn Tag

Trigger hoạt động khi khách hàng được gắn một tag theo chỉ định. Các hành động sẽ thực hiện với khách hàng đó.

Trigger được kích hoạt cho một khách hàng bằng cách:

* Bạn tự cập nhật thủ công tag của khách hàng tại phần chi tiết khách hàng
* Tag của khách hàng được gắn tự động khi được thực hiện hành động Gắn tag cho khách hàng ở Flow khác, Sequence, Campaign.

{% hint style="info" %}
Trigger chỉ hoạt động khi đã kích hoạt. Chỉ có thể kích hoạt trigger khi Flow đã xuất bản.

Trigger hoạt động với những khách hàng được gắn tag ngay sau khi kích hoạt trigger.
{% endhint %}

1. **Tìm và chọn Trigger Được gắn Tag.**

<figure><img src="https://lh6.googleusercontent.com/z16e3Xl2IQy2TRzDrEsesMTjtjcvCH13ufTk4T5cNbksAdKHxjCH48w0NXJHDUjLfy__6AXadp8u3Isl_6CvHipmAe8wVil1v26EzLLaJGjwGF7sYhacf0BGZJEQGuJevMhttf2R-3tlKAy8pNTNT-I" alt=""><figcaption></figcaption></figure>

2. **Thêm điều kiện kích hoạt Trigger nếu có**, xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").

<figure><img src="https://lh3.googleusercontent.com/KDuGg-4CQcwTlSCxIiI5a8vO_VIQ7EJ4nyj486blJB8SP1q9OEzhjXFe1FU3enBAOTfLRKXjy1w3M2cp0Lwf3wCIVIbqa5wpO_6UslA2zkxXj5Hd51r9KAXBLg-Nx3zmdfmzImT3Gm3azZ85PJjQm9M" alt=""><figcaption></figcaption></figure>

3.  **Chọn tag khách hàng kích hoạt trigger** từ danh sách Tag. Bạn có thể làm mới danh sách hoặc tìm kiếm tag theo tên. \


    <figure><img src="../../../.gitbook/assets/Chon tag.gif" alt="" width="563"><figcaption><p>Chọn Tag</p></figcaption></figure>



    <figure><img src="../../../.gitbook/assets/LadiFlow _ Customer Engagement Platform - Automation - Google Chrome 2024-05-16 13-29-28 (1).gif" alt="" width="563"><figcaption><p>Thêm mới nhanh tag</p></figcaption></figure>
4.  **Chọn tần suất chạy Flow**: 1 lần hoặc lặp lại. \


    <figure><img src="../../../.gitbook/assets/image (684).png" alt="" width="474"><figcaption></figcaption></figure>

{% hint style="info" %}
Nếu chọn MỘT LẦN, flow sẽ chỉ chạy 1 lần khi lần đầu khách hàng được gắn Tag đã chọn, sau khi xoá tag và gán lại flow sẽ không hoạt động với khách hàng đó.&#x20;

Nếu chọn LẶP LẠI, flow sẽ chạy bất cứ khi nào khách hàng được gắn Tag đã chọn.
{% endhint %}

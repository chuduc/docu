---
description: Sự kiện khi xoá tag khách hàng
---

# Khi một ai đó được Xóa Tag

Trigger hoạt động khi khách hàng bị xoá Tag đã cài đặt khi khách hàng đã được gắn tag này trước đó. Các hành động sẽ thực hiện với khách hàng đó.

Trigger được kích hoạt cho một khách hàng bằng cách:

* Bạn tự xoá thủ công tag của khách hàng tại phần chi tiết khách hàng.
* Tag của khách hàng được xoá tự động khi được thực hiện hành động **Xoá tag** cho khách hàng ở Flow khác, Sequence, Campaign.

{% hint style="info" %}
Trigger chỉ hoạt động khi đã kích hoạt. Chỉ có thể kích hoạt trigger khi Flow đã xuất bản.

Trigger hoạt động với những khách hàng bị xoá tag đã cài đặt.
{% endhint %}

\
1\.  **Tìm và chọn Trigger Bị xoá Tag.**

<figure><img src="https://lh4.googleusercontent.com/zMu6TsqQZTvxdwVY5DjzuYGoWltfWabi2_gfBEGPntSfq6ahtHNnbm0n-5kUIM0qKL7dgSSZW7JLL_VFdvRfxh5GVh6n2EBdhZM5Z2va7JdHBmF5a3bzjxEcup1tlh4F-5xOhLtVkm0M_1u4NePYCqs" alt=""><figcaption></figcaption></figure>

2. Chọn điều kiện kích hoạt trigger nếu muốn giới hạn tập khách hàng của flow, xem thêm tại [them-dieu-kien-kich-hoat-trigger.md](them-dieu-kien-kich-hoat-trigger.md "mention").
3.  **Chọn tag khách hàng kích hoạt Trigger**. Bạn có thể làm mới danh sách hoặc tìm kiếm để tìm tag mong muốn.\


    <figure><img src="../../../.gitbook/assets/image (685).png" alt="" width="476"><figcaption></figcaption></figure>
4. **Chọn Tần suất chạy Flow**: 1 lần hay lặp lại.
   * Nếu chọn lặp lại Flow sẽ chạy khi tag đó được xoá.
   *   Nếu chọn 1 lần, flow sẽ chỉ chạy lần đầu tag đó được xoá.\


       <figure><img src="../../../.gitbook/assets/image (686).png" alt="" width="475"><figcaption></figcaption></figure>

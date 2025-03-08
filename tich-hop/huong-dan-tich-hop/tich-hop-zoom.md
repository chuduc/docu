# Tích hợp Zoom

### Tạo ứng dụng trên Zoom

1. Truy cập vào đường dẫn [https://marketplace.zoom.us/](https://marketplace.zoom.us/)
2. Đăng nhập tài khoản zoom của bạn
3. Chọn **Develop**, sau đó chọn **Build App**

<figure><img src="../../.gitbook/assets/image (447).png" alt="" width="426"><figcaption></figcaption></figure>

4. Chọn **Server to Server OAuth App** và chọn **Create**

<figure><img src="../../.gitbook/assets/image (826).png" alt="" width="563"><figcaption></figcaption></figure>

5. **Nhập App Name** và chọn **Create.**

<figure><img src="../../.gitbook/assets/image (827).png" alt="" width="490"><figcaption></figcaption></figure>

Được kết quả như sau:

<figure><img src="../../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>

6. **Điền thông tin tab Information.**

<figure><img src="../../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>

7. **Chuyển tab Scope và chọn Add scope.**

<figure><img src="../../.gitbook/assets/image (830).png" alt=""><figcaption></figcaption></figure>

8. **Tích chọn đủ các scope sau**:

* View a meeting / meeting:read:meeting:admin

<figure><img src="../../.gitbook/assets/image (831).png" alt="" width="563"><figcaption></figcaption></figure>

* View a user's meetings / meeting:read:list\_meetings:admin

<figure><img src="../../.gitbook/assets/image (851).png" alt="" width="556"><figcaption></figcaption></figure>

* Create a meeting for a user / meeting:write:meeting:admin

<figure><img src="../../.gitbook/assets/image (832).png" alt="" width="557"><figcaption></figcaption></figure>

* View a webinar / webinar:read:webinar:admin

<figure><img src="../../.gitbook/assets/image (833).png" alt="" width="563"><figcaption></figcaption></figure>

* View a user's webinars / webinar:read:list\_webinars:admin

<figure><img src="../../.gitbook/assets/image (852).png" alt="" width="551"><figcaption></figcaption></figure>

* Create a webinar for a user / webinar:write:webinar:admin

<figure><img src="../../.gitbook/assets/image (834).png" alt="" width="554"><figcaption></figcaption></figure>

* View a user / user:read:user:admin

<figure><img src="../../.gitbook/assets/image (835).png" alt="" width="554"><figcaption></figcaption></figure>

9. Chọn **Continue** để tiếp tục.

<figure><img src="../../.gitbook/assets/image (836).png" alt=""><figcaption></figcaption></figure>

10. Chọn **Activate** your app.

<figure><img src="../../.gitbook/assets/image (837).png" alt=""><figcaption></figcaption></figure>

Kết quả sẽ như sau:

<figure><img src="../../.gitbook/assets/image (838).png" alt=""><figcaption></figcaption></figure>

### Tích hợp Zoom trên LadiFlow

1. Truy cập LadiFlow, mở mục **Tích hợp**, tìm và chọn ứng dụng **Zoom.**

<figure><img src="../../.gitbook/assets/zoom.png" alt=""><figcaption></figcaption></figure>

2. Nhập Tên tích hợp.
3. Chọn **Thêm liên kết** và điền các thông tin vào Form như sau:

* Lấy thông tin Account ID, Client ID, Client Secret, Secret Token lấy trên tab App Credentials:

<figure><img src="../../.gitbook/assets/image (839).png" alt=""><figcaption></figcaption></figure>

* Copy Secret Token từ tab Feature:

<figure><img src="../../.gitbook/assets/image (840).png" alt=""><figcaption></figcaption></figure>

4. Chọn **Lưu liên kết** để hoàn thành thêm mới tích hợp.

### Thêm webhook vào ứng dụng trên Zoom

1. Mở mục **Feature**, sau đó chọn bật **Event Subscriptions.**\


<figure><img src="../../.gitbook/assets/image (842).png" alt=""><figcaption></figcaption></figure>

2. Chọn **Add Event Subscription.**

<figure><img src="../../.gitbook/assets/image (843).png" alt=""><figcaption></figcaption></figure>

3. Chọn **Add Events** và **tích chọn các mục** như hìn&#x68;**:**

<figure><img src="../../.gitbook/assets/image (844).png" alt="" width="563"><figcaption></figcaption></figure>

* Meeting:&#x20;

<figure><img src="../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

* Webinar:

<figure><img src="../../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>

4. Chọn **Done.**
5. Trên LadiFlow chọn tích hợp của tôi, mở tích hợp Zoom bạn vừa tạo.
6. Chọn sao chép **Url Webhook.**

<figure><img src="../../.gitbook/assets/image (487).png" alt="" width="561"><figcaption></figcaption></figure>

7. Dán Url Webhook vừa sao chép, dán vào mục **Event notification endpoint URL.** Sau đó chọn **Validate**.

<figure><img src="../../.gitbook/assets/validate url.png" alt="" width="345"><figcaption></figcaption></figure>

8. Sau khi validate thành công, bạn **chọn Save** để lưu lại.

**Hiện tại hệ thống không giới hạn số tích hợp Zoom.**

\

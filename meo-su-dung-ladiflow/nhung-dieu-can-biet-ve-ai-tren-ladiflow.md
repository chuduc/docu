# Những điều cần biết về AI trên LadiFlow

LadiFlow đã tích hợp AI với công nghệ ChatGPT mới nhất do OpenAI cung cấp. Bạn có thể sử dụng tính năng Tạo email bằng AI, tạo nội dung bằng AI. AI sẽ giúp bạn tạo ra nội dung, email dựa theo yêu cầu mong muốn của bạn.

{% hint style="info" %}
Tính năng liên quan đến AI yêu cầu tài khoản trả phí có gói từ Standard trở lên&#x20;
{% endhint %}

Khi bạn sử dụng Tạo email bằng AI, Tạo nội dung bằng AI hệ thống sẽ trừ phí dựa theo lượng nội dung nhập vào và nội dung AI đã tạo.

<figure><img src="../.gitbook/assets/image (651).png" alt="" width="360"><figcaption></figcaption></figure>

### Công thức tính chi phí&#x20;

Công thức tính chi phí sử dụng các tính năng liên quan đến AI trên LadiFlow như sau:

$$
T = Tổng Số Token/1000
$$

Gọi X là phần nguyên của T:

$$
X= [T]
$$

Gọi Z là phần thập phân của T

$$
Z=\lbrace T\rbrace
$$

Công thức tính số credit đã tiêu cho hành động Tạo Email AI và Tạo nội dung AI như sau:

$$
Số Credit = \begin{cases}
   0.03*X+0.02 &\text{if } Z \le 0.5\\
   0.03*(X+1)  &\text{if } Z \gt 0.5 
\end{cases}
$$

Ví dụ: Tổng số token hệ thống ghi nhận là 1034

\=> T=1.034 ; X= 1; Z=0.034

\=> Số credit đã bị trừ = 0.03 \* 1 +0.02 = 0.05

### Token là gì? Làm sao để kiểm tra số token đã ghi nhận trên LadiFlow

Token trong OpenAI được định nghĩa là những từ, cụm từ mà OpenAI xác định được theo các Model của họ. Trước khi đoạn văn được AI thực hiện sẽ được chia thành các token. Thông thường token sẽ được tính như sau:

* 100 tokens \~= 75 từ&#x20;
* 1-2 câu \~= 30 token
* 1 đoạn văn \~= 100 token
* 1,500 từ \~= 2048 token

**Token đầu vào:** Là số token được xác định từ dữ liệu bạn nhập vào.

**Token đầu ra:** Là số token từ dữ liệu mà AI trả về cho bạn.

Tuy nhiên, phụ thuộc vào từng Model và từng lần nhập, câu văn mà OpenAI sẽ xác định số lượng Token khác nhau. Bạn có thể kiểm tra số lượng token trong câu văn tại [https://platform.openai.com/tokenizer](https://platform.openai.com/tokenizer). Tuy nhiên kết quả có có tính tương đối và phụ thuộc vào Model, ngôn ngữ trong nội dung của bạn.

### Mẹo sử dụng công cụ AI trên LadiFlow hiệu quả?

Công cụ AI trên LadiFlow sử dụng công nghệ của ChatGPT, do đó để AI tạo ra đúng nội dung bạn mong muốn hãy mô tả đúng trọng tâm, chi tiết. Bạn có thể trả lời các câu hỏi sau trước khi nhập nội dung để AI thực hiện:

* Bạn mong muốn AI tạo ra nội dung gì?
* Nội dung chính của tin nhắn, thông điệp là gì?
* Yêu cầu đặc biệt nào cho tin nhắn, thông điệp không?
* Đối tượng nhận tin nhắn, thông điệp là ai?
* Nội dung kêu gọi hành động là gì?

**Lưu ý**: Hạn chế sử dụng nhiều ngôn ngữ khác nhau, từ viết tắt, từ lóng, từ địa phương, viết sai chính tả... để AI hiểu được đúng mong muốn của bạn.

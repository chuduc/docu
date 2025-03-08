# Giải thích các Toán tử trong điều kiện và cách áp dụng

Khi bạn làm việc với dữ liệu khách hàng, xây dựng kịch bản chắc hẳn bạn đã từng sử dụng các công cụ bộ lọc, điều kiện trên LadiFlow. Tuy nhiên để xây dựng và áp dụng bộ lọc theo đúng bài toán và nhu cầu  không hề dễ thực hiện. Bài viết này sẽ giúp bạn hiểu rõ từng toán tử và cách áp dụng kết hợp các biểu thức phù hợp với nhu cầu thực tế.

### Toán tử trên LadiFlow là gì?

Toán tử trên LadiFlow là biểu thức logic( lớn hơn, nhỏ hơn, bằng, chứa...) dùng để so sánh, áp dụng trong biểu thức, là điều kiện để lọc ra tập dữ liệu thỏa mãn biểu thức.\


<figure><img src="../.gitbook/assets/image (761).png" alt="" width="319"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (760).png" alt="" width="563"><figcaption></figcaption></figure>

Tương ứng với từng kiểu dữ liệu sẽ có những biểu thức logic tương ứng. Kiểu dữ liệu bao gồm: dòng văn bản, dạng số, dạng danh sách, boolean, hộp chọn, hộp kiểm....

### Giải thích từng toán tử

Trước hết, để bạn hiểu rõ định nghĩa từng toán tử, tôi sẽ đưa ra các định nghĩa sau:

*   **Trường so sánh**: Là trường thông tin trong biểu thức điều kiện dùng để so sánh với Giá trị so sánh theo toán tử với công thức: \<Trường so sánh> \<toán tử> \<Giá trị so sánh>. Đây là các trường trong dữ liệu khách hàng.\


    <figure><img src="../.gitbook/assets/image (756).png" alt="" width="324"><figcaption><p>Trường so sánh trong hành động Điều kiện</p></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (757).png" alt="" width="243"><figcaption><p>Trường so sánh trong bộ lọc nâng cao</p></figcaption></figure>
* **Giá trị so sánh**: là giá trị dùng để so sánh với Trường so sánh theo toán tử.

<figure><img src="../.gitbook/assets/image (758).png" alt="" width="241"><figcaption><p>Giá trị so sánh trong bộ lọc nâng cao</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (759).png" alt="" width="317"><figcaption><p>Giá trị so sánh trong hành động Điều kiện</p></figcaption></figure>

<table><thead><tr><th width="158">Toán tử</th><th>Mô tả</th></tr></thead><tbody><tr><td>Là, Đúng bằng</td><td>Trả ra kết quả Trường so sánh có giá trị chính xác( Bằng) với giá trị nhập</td></tr><tr><td>Không phải là</td><td>Trả ra kết quả Trường so sánh có giá trị khác với giá trị nhập. </td></tr><tr><td>Có bất kỳ giá trị nào</td><td>Trả ra kết quả Trường so sánh có giá trị, tất cả các giá trị đều thỏa mãn.  <br>Có bất kỳ giá trị nào + Không có giá trị= Tập khách hàng của bạn.</td></tr><tr><td>Chứa</td><td><p>Trả ra kết quả Trường so sánh có giá trị chứa Giá trị so sánh. Bạn cần nhập giá trị so sánh theo từ, cụm từ. Với kiểu dữ liệu danh sách, điều kiện áp dụng với từng phần tử trong dánh sách.<br>Ví dụ:<br> "Nguyễn Văn A" chứa "Văn A" => true</p><p>"Nguyễn Văn A" chứa "Văn B" =>false<br>"Nguyễn Văn A" chứa "Vă"=>false</p></td></tr><tr><td>Không chứa</td><td><p>Trả ra kết quả Trường so sánh có giá trị không chứa Giá trị so sánh. Bạn cần nhập giá trị so sánh theo từ, cụm từ. Với kiểu dữ liệu danh sách, điều kiện áp dụng với từng phần tử trong dánh sách.<br>Ví dụ: <br>"Nguyễn Văn A" Không chứa "Văn A" => false</p><p>"Nguyễn Văn A" chứa "Văn B" =>false<br>"Nguyễn Văn A" chứa "Vă"=>false</p></td></tr><tr><td>Bắt đầu với</td><td>Trả ra kết quả Trường so sánh có giá trị Bắt đầu với Giá trị so sánh. <br>Ví dụ: <br>"Nguyễn Văn A" Bắt đầu với "Nguyễn"=> true<br>"Nguyễn Văn A" Bắt đầu với "Nguyen" =>false<br>"Nguyễn Văn A" Bắt đầu với "Nguy"=>true<br>"Nguyễn Văn A" Bắt đầu với "Nguyễn" =>true</td></tr><tr><td>Không có giá trị</td><td>Trả ra kết quả Trường so sánh không có bất kỳ giá trị nào. Ví dụ bạn tạo mới trường tùy chỉnh thì tất cả khách hàng đang có Không có giá trị hoặc bạn xóa hết dữ liệu trong trường dữ liệu và cập nhật khách hàng. Khi xem thông tin khách hàng thì trường dữ liệu này Không có giá trị.<br>Không có giá trị + Có bất kỳ giá trị nào = Tập khách hàng của bạn</td></tr><tr><td>Lớn hơn</td><td>Trả ra kết quả Trường so sánh lớn hơn Giá trị so sánh. Chỉ áp dụng với kiểu dữ liệu dạng số và ngày tháng.<br>Đối với kiểu dữ liệu ngày tháng, bạn xem thêm tại mục</td></tr><tr><td>Lớn hơn hoặc bằng</td><td>Trả ra kết quả Trường so sánh lớn hơn hoặc bằng Giá trị so sánh. Chỉ áp dụng với kiểu dữ liệu dạng số.</td></tr><tr><td>Nhỏ hơn</td><td>Trả ra kết quả Trường so sánh nhỏ hơn Giá trị so sánh. Chỉ áp dụng với kiểu dữ liệu dạng số và ngày tháng.<br>Đối với kiểu dữ liệu ngày tháng, bạn xem thêm tại mục</td></tr><tr><td>Nằm trong list</td><td>Trả ra kết quả Trường so sánh có giá trị nằm trong danh sách. Chỉ áp dụng với kiểu dữ liệu dòng văn bản, dạng số, hộp chọn, tự tăng.<br>Ví dụ: <br>"A" nằm trong list ["A","B","C"] =>true<br>"A" nằm trong list ["B","C","D"] =>false</td></tr><tr><td>Nhỏ hơn hoặc bằng</td><td>Trả ra kết quả Trường so sánh nhỏ hơn hoặc bằng Giá trị so sánh. Chỉ áp dụng với kiểu dữ liệu dạng số.</td></tr></tbody></table>

### Toán tử với kiểu dữ liệu ngày tháng

<table><thead><tr><th width="161">Toán tử</th><th>Mô tả</th></tr></thead><tbody><tr><td>Là ngày</td><td>Trả ra kết quả Trường so sánh Bằng Giá trị so sánh. Giá trị so sánh là ngày cụ thể</td></tr><tr><td>Từ ngày</td><td>Trả ra kết quả Trường so sánh bắt đầu từ Giá trị so sánh tới tương lai. Giá trị so sánh là ngày cụ thể</td></tr><tr><td>Trước ngày hiện tại</td><td>Trả ra kết quả Trường so sánh nhỏ hơn ngày hiện tại. Các giá trị ngày trong quá khứ sẽ thỏa mãn điều kiện.</td></tr><tr><td>Sau ngày hiện tại</td><td>Trả ra kết quả Trường so sánh lớn hơn ngày hiện tại. Các giá trị ngày trong tương lai sẽ thỏa mãn điều kiện.</td></tr><tr><td>Đến ngày</td><td>Trả ra kết quả Trường so sánh nhỏ hơn hoặc bằng Giá trị so sánh. Giá trị so sánh là ngày cụ thể. Các giá trị là quá khứ của Giá trị so sánh thỏa mãn điều kiện</td></tr><tr><td>Có bất kỳ giá trị nào</td><td>Trả ra kết quả Trường so sánh có giá trị.<br>Có bất ký giá trị nào + Không có giá trị = Tập khách hàng</td></tr><tr><td>Không có giá trị</td><td>Trả ra kết quả trường so sánh không có giá trị.</td></tr><tr><td>Lớn hơn</td><td>Trả ra kết quả trường so sánh lớn hơn bao nhiêu ngày trước.<br>Ví dụ: Ngày tái khám lớn hơn 5 ngày trước => Ngày tái khám > (Ngày hiện tại - 5 ngày)</td></tr><tr><td>Nhỏ hơn</td><td>Trả ra kết quả trường so sánh nhỏ hơn bao nhiều ngày trước.<br>Ví dụ: Ngày tái khám nhỏ hơn 5 ngày trước => Ngày tái khám &#x3C;(Ngày hiện tại -5 ngày)</td></tr><tr><td>Cách đây</td><td>Trả ra kết quả trường so sánh cách đây bao nhiêu ngày trước.<br>Ví dụ: Ngày tái khám cách đây 5 ngày trước=> Ngày tái khám= Ngày hiện tại - 5 ngày</td></tr></tbody></table>

{% hint style="info" %}
Với kiểu dữ liệu thời gian, thời gian trong tương lai luôn lớn hơn thời gian ở hiện tại và quá khứ.
{% endhint %}

### Cách áp dụng kết hợp các điều kiện

Kết hợp các điều kiện giúp bạn Segment tập khách hàng mong muốn, lọc ra danh sách khách hàng hoặc là điều kiện lọc khách hàng vào Flow. Mỗi chương trình, kịch bản sẽ có các điều kiện khác nhau. Do đó bạn cần kết hợp linh hoạt các điều kiện để thực hiện kịch bản mong muốn. Các bước cần thực hiện như sau:

1. **Xác định điều kiện/tập điều kiện thực hiện kịch bản**: ví dụ Khách hàng có tổng giá trị lớn hơn 1 triệu đồng và có sinh nhật vào tháng 5.
2. **Phân tách điều kiện ở bước 1 thành các điều kiện đơn lẻ(không thể phân tách được nữa) và mối quan hệ giữa các điều kiện.** Cần ứng dụng linh hoạt theo toán tử trên LadiFlow.\
   Ví dụ ở bước 1, ta xác định được 2 điều kiện đơn lẻ sau:\
   \- Điều kiện 1: Tổng giá trị đơn hàng > 1 triệu\
   \- Điều kiện 2: Tháng sinh = 5\
   \- Mối quan hệ giữa các điều kiện: VÀ( Tất cả điều kiện)
3. **Thực hiện rút gọn các điều kiện nếu các điều kiện giao nhau hoặc trùng nhau**. Việc rút gọn điều kiện sẽ giúp điều kiện của bạn ngắn gọn, dễ hiểu và dễ quản lý.\
   Ví dụ:\
   \- Điều kiện 1: Thời gian tạo đơn cuối < 2 tháng\
   \- Điều kiện 2: Thời gian tạo đơn cuối < 1 năm\
   \- Mối quan hệ giữa các điều kiện: OR(Một trong các điều kiện)\
   \=> Ta rút gọn điều kiện: Thời gian tạo đơn cuối <1 năm
4. **Kiểm tra và đảm bảo các dữ liệu trên tài khoản của bạn đã có**. Nếu chưa có hãy thực hiện bổ sung bằng cách import file, tạo các flow để bổ sung dữ liệu...
5. **Áp dụng điều kiện** vào các khu vực cần sử dụng: Tạo segment, lọc danh sách khách hàng, Hành động điều kiện trong Flow...

Để hiểu rõ cách làm, bạn theo dõi 2 ví dụ dưới đây:

**VÍ DỤ 1: Khách hàng có hạng là Gold với tổng chi tiêu lớn hơn hoặc bằng 2 triệu hoặc khách hàng có hạng Diamond với tổng chi tiêu lớn hơn hoặc bằng 4 triệu thì gửi voucher giảm giá**

1. Điều kiện thực hiện kịch bản: Khách hàng có hạng là Gold với tổng chi tiêu lớn hơn hoặc bằng 2 triệu hoặc khách hàng có hạng Diamond với tổng chi tiêu lớn hơn hoặc bằng 4 triệu
2. Tách thành các tập điều kiện đơn lẻ sau:\
   &#x20;Nhóm điều kiện 1:  Hạng là Gold và tổng giá trị đơn hàng lớn hơn hoặc bằng 2 triệu

Nhóm điều kiện 2: Hạng là Diamond và tổng giá trị đơn hàng lớn hơn hoặc bằng 4 triệu

Mối quan hệ giữa các nhóm điều kiện: OR(Một trong các điều kiện)

3. Các điều kiện không giao nhau, trùng nhau nên không thể rút gọn.
4.  Kiểm tra dữ liệu Hạng và tổng chi tiêu đã có trên khách hàng của bạn chưa\
    \- **Dữ liệu Hạng**: nếu thông tin khách hàng chưa có, hãy kiểm tra các mã trường tùy chỉnh tại nền tảng tích hợp đổ dữ liệu khách hàng(nếu có), danh sách các mã trường dữ liệu đã được liệt kê trên help của từng nền tảng tích hợp. Nếu có mã dữ liệu hạng thành viên, hãy tạo mã trường tùy chỉnh tương ứng. Nếu không có, cần nhập file dữ liệu bổ sung hoặc chạy kịch bản bổ sung dữ liệu.\
    \- **Dữ liệu tổng chi tiêu**: Tổng chi tiêu là trường dữ liệu Tổng giá trị đơn hàng

    <figure><img src="../.gitbook/assets/image (770).png" alt="" width="563"><figcaption><p>Mã trường tùy chỉnh hạng khách hàng trên Nhanhvn</p></figcaption></figure>


5. Thực hiện tạo thiết lập điều kiện trong Segment.

Ở đây, ta thấy có 2 nhóm điều kiện nên cần sử dụng tính năng segment để lọc tập khách hàng. Sau khi thết lập, điều kiện segment sẽ như sau:

<figure><img src="../.gitbook/assets/image (771).png" alt="" width="454"><figcaption></figcaption></figure>

Để xem danh sách khách hàng thuộc segment này, bạn chọn Segment tại danh sách khách hàng như hình dưới đây:

<figure><img src="../.gitbook/assets/image (772).png" alt="" width="563"><figcaption></figcaption></figure>

Sau khi đã có segment, bạn có thể chạy Campaign với tập này, hoặc thực hiện Flow với các Khách hàng trong segment.

**VÍ DỤ 2**: **Khách hàng sinh nhật tháng 5 và có đơn cuối cùng từ tháng 1/2024 đến hết tháng 4/2024 thì gửi voucher khuyến mại**

1. Điều kiện khách hàng: Khách hàng sinh nhật tháng 5 và có đơn cuối cùng từ tháng 1/2024 đến hết tháng 4/2024
2. Phân tách điều kiện thành các điều kiện đơn lẻ:\
   \- Điều kiện 1: Tháng sinh là 5\
   \- Điều kiện 2: Ngày tạo đơn cuối từ ngày 0:00 01/01/2024\
   \- Điều kiện 3: Ngày tạo đơn cuối đến ngày 24:00 30/04/2024, tương đương với 0:00 01/05/2024\
   \- Mối quan hệ giữa các điều kiện: Và(Tất cả điều kiện)
3. Các điều kiện không giao nhau, nên không thể rút gọn.
4. Tìm các trường thông tin theo điều kiện\
   \- Tháng sinh tương ứng với trường Tháng sinh\
   \- Ngày tạo đơn cuối tương ứng với trường Order Created At
5. Thực hiện tạo Segment, bộ lọc dữ liệu ta được kết quả sau

<figure><img src="../.gitbook/assets/image (773).png" alt="" width="563"><figcaption></figcaption></figure>

### Các biểu thức logic trong Trigger Trường tùy chỉnh thay đổi và Trigger Trường mặc định thay đổi

<table><thead><tr><th width="166"></th><th></th></tr></thead><tbody><tr><td>Đã thay đổi và bằng</td><td>Trường so sánh thay đổi giá trị và giá trị mới bằng Giá trị so sánh.</td></tr><tr><td>Đã thay đổi và chứa</td><td><p>Trường so sánh đã thay đổi giá trị và giá trị mới chứa Giá trị so sánh. Bạn cần nhập giá trị so sánh theo từ, cụm từ. Với kiểu dữ liệu danh sách, điều kiện đúng khi một phần tử trong danh sách thỏa mãn.<br>Ví dụ:<br> "Nguyễn Văn A" chứa "Văn A" => true</p><p>"Nguyễn Văn A" chứa "Văn B" =>false<br>"Nguyễn Văn A" chứa "Vă"=>false</p></td></tr><tr><td>Đã thay đổi và không bằng</td><td>Trường so sánh đã thay đổi giá trị và giá trị mới Khách với Giá trị so sánh.</td></tr><tr><td>Đã thay đổi và không chứa</td><td>Trường so sánh đã thay đổi giá trị và giá trị mới KHÔNG chứa Giá trị so sánh. Bạn cần nhập giá trị so sánh theo từ, cụm từ. Với kiểu dữ liệu danh sách, điều kiện đúng khi tất cả phần tử trong danh sách thỏa mãn.</td></tr><tr><td>Đã thay đổi và bắt đầu với </td><td>Trường so sánh đã thay đổi giá trị và giá trị mới bắt đầu với Giá trị so sánh.<br>Ví dụ: <br>"Nguyễn Văn A" Bắt đầu với "Nguyễn"=> true<br>"Nguyễn Văn A" Bắt đầu với "Nguyen" =>false<br>"Nguyễn Văn A" Bắt đầu với "Nguy"=>true<br>"Nguyễn Văn A" Bắt đầu với "Nguyễn" =>true</td></tr><tr><td>Đã thay đổi và thành Không có giá trị</td><td>Trường so sánh đã thay đổi giá trị thành không có giá trị. Khi xem thông tin khách hàng thì trường dữ liệu này Không có giá trị.</td></tr><tr><td>Đã thay đổi và nằm trong list</td><td>Trường so sánh đã thay đổi giá trị và giá trị mới nằm trong danh sách. Chỉ áp dụng với kiểu dữ liệu dòng văn bản, dạng số, hộp chọn, tự tăng.<br>Ví dụ: <br>"A" nằm trong list ["A","B","C"] =>true<br>"A" nằm trong list ["B","C","D"] =>false</td></tr><tr><td>Đã thay đổi và thành giá trị bất kỳ</td><td>Trường so sánh đã thay đổi giá trị và giá trị mới có dữ liệu. </td></tr><tr><td>Đã thay đổi và lớn hơn</td><td>Trường so sánh đã thay đổi và giá trị mới lớn hơn giá trị so sánh</td></tr><tr><td>Đã thay đổi và nhỏ hơn</td><td>Trường so sánh đã thay đổi và giá trị mới nhỏ hơn giá trị so sánh</td></tr></tbody></table>

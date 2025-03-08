# Xem tổng chi phí của Flow/Campaign/Sequence

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/sequence/subscribe](https://api.service.ladiflow.com/1.0/sequence/subscribe)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/flow/get-cost' \
--header 'Api-Key: {API-KEY}' \
--header 'Content-Type: text/plain' \
--data '{
    "from_date": "2024-04-09T17:00:00.610Z",
    "to_date": "2024-05-10T16:59:59.611Z",
    "type": "MESSAGE",
    "source": "FLOW",
    "flow_id": null,
    "trigger_id": null,
    "flow_config_id": null,
    "campaign_id": null,
    "sequence_id": null
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>from_date</td><td>string</td><td>Có</td><td>Thời gian bắt đầu lấy dữ liệu</td></tr><tr><td>to_date</td><td>string</td><td>Không</td><td>Thời gian kết thúc lấy dữ liệu</td></tr><tr><td>type</td><td>string</td><td>Không</td><td>Mã hành động muốn xem chi phí. Xem danh sách loại hành động tại <a data-mention href="./#danh-sach-ma-hanh-dong-cua-flow-campaign-sequence">#danh-sach-ma-hanh-dong-cua-flow-campaign-sequence</a></td></tr><tr><td>source</td><td>string</td><td>Có</td><td>Loại chiến dịch: <br>- FLOW<br>- CAMPAIGN<br>- SEQUENCE</td></tr><tr><td>flow_id</td><td>string</td><td>Không</td><td>ID của Flow<br>Nếu có giá trị ID flow thì source = FLOW</td></tr><tr><td>trigger_id</td><td>string</td><td>Không</td><td>ID của trigger trong flow<br>Nếu có giá trị ID trigger thì source=Flow và có giá trị flow_id</td></tr><tr><td>flow_config_id</td><td>string</td><td>Không</td><td>ID của hành động trong flow<br>Nếu có giá trị ID trigger thì source=Flow và có giá trị flow_id</td></tr><tr><td>campaign_id</td><td>string</td><td>Không</td><td>ID của Campaign<br>Nếu có giá trị ID flow thì source = CAMPAIGN</td></tr><tr><td>sequence_id</td><td>string</td><td>Không</td><td>ID của Sequence<br>Nếu có giá trị ID flow thì source = SEQUENCE</td></tr></tbody></table>

#### Example response

```json
{
    "data": {
        "total_credits": 81,
        "total_money": 0
    },
    "message": "Thành công",
    "code": 200
}
```

#### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả                                                                 |
| ---------- | ------------ | --------------------------------------------------------------------- |
| data       | Object       | <p>total_credits: số điểm đã tiêu<br>total_money: số tiền đã tiêu</p> |
| message    | string       | Thông điệp                                                            |
| code       | number       | Mã phản hồi                                                           |

---
description: Đăng ký sequence cho khách hàng
---

# Đăng ký sequence

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/sequence/subscribe](https://api.service.ladiflow.com/1.0/sequence/subscribe)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/sequence/subscribe' \
--header 'Api-Key: {{API-KEY}}' \
--data-raw '{
    "email": "test@gmail.com",
    "custom_fields": [
        {
        "name": "ldp_pkg_name",
        "value": "LADIPAGE-PRO"
        },
        {
        "name": "ldp_pkg_name1",
        "value": "LADIPAGE-PRO"
        }
    ],
    "external_data": [
        {
        "name": "name1",
        "value": "Value1"
        },
        {
        "name": "name2",
        "value": "Value2"
        }
    ],
    "sequence_id": "YOUR_SEQUENCEID"
}'

```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>email</td><td>string</td><td>có</td><td>email của khách hàng</td></tr><tr><td>sequence_id</td><td>string</td><td>có</td><td>ID của sequence</td></tr><tr><td>custom_fields</td><td>List Object</td><td></td><td>Dữ liệu trường tuỳ chỉnh</td></tr><tr><td>external_data</td><td>List Object</td><td></td><td>Dữ liệu bổ sung</td></tr></tbody></table>

#### Example response

```json
{
    "data": {},
    "message": "Thành công",
    "code": 200
}
```

#### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả       |
| ---------- | ------------ | ----------- |
| data       | Object       |             |
| message    | string       | Thông điệp  |
| code       | number       | Mã phản hồi |

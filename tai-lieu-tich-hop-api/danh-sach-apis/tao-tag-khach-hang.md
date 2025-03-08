# Tạo Tag khách hàng

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/customer/create-tag](https://api.service.ladiflow.com/1.0/customer/create-tag)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/customer/create-tag' \
--header 'Api-Key: {Api-Key}' \
--header 'Content-Type: application/json' \
--data '{
    "name": "Test"
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>name</td><td>string</td><td></td><td>Tên tag</td></tr></tbody></table>

### Example response

```json
{
 "data": {
   tag_id: ""
 },
 "message": "Thành công",
 "code": 200
}
```

### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả       |
| ---------- | ------------ | ----------- |
| data       | Object       | Dữ liệu tag |
| message    | string       | Thông điệp  |
| code       | number       | Mã phản hồi |

# Danh sách Sequence

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/sequence/list](https://api.service.ladiflow.com/1.0/sequence/list)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/sequence/list' \
--header 'Api-Key: {{API-key}}' \
--header 'Content-Type: application/json' \
--data '{
    "keyword":null,
    "page": 1,
    "limit": 3
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>keyword</td><td>string</td><td></td><td>từ khoá tìm kiếm</td></tr><tr><td>page</td><td>Number</td><td></td><td>Số trang<br>Mặc định =1</td></tr><tr><td>limit</td><td>Number</td><td></td><td>Số lượng bản ghi/request<br>Mặc định =20</td></tr></tbody></table>

### Example response

```json

{
    "data": {
        "total": 48,
        "limit": 3,
        "items": [
            {
                "id": "653a0e050217d10012313bce",
                "name": "[kun] test sequence #1111",
                "tags": [],
                "created_at": "2023-10-26T06:58:13.196Z",
                "updated_at": "2023-10-27T01:53:13.223Z"
            },
            {
                "id": "653876e9d32ef300126aba68",
                "name": "dddddđ",
                "tags": [],
                "created_at": "2023-10-25T02:01:13.967Z",
                "updated_at": "2023-10-26T10:02:09.404Z"
            },
            {
                "id": "65376fb1bce6af00127f1bab",
                "name": "[huê] đa kênh",
                "tags": [],
                "created_at": "2023-10-24T07:18:09.879Z",
                "updated_at": "2023-10-27T01:24:26.469Z"
            }
        ]
    },
    "message": "Thành công",
    "code": 200
}
```

### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả       |
| ---------- | ------------ | ----------- |
| data       | Object       |             |
| message    | string       | Thông điệp  |
| code       | number       | Mã phản hồi |

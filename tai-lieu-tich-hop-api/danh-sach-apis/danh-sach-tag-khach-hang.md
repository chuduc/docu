---
description: Lấy danh sách Tags của khách hàng
---

# Danh sách Tag khách hàng

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/customer/list-tag](https://api.service.ladiflow.com/1.0/customer/list-tag)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/customer/list-tag' \
--header 'Api-Key: {{API_KEY}}' \
--data '{
    "limit": 20,
    "page": 0,
    "keyword": "test"
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>limit</td><td>number</td><td></td><td>Số bản ghi giới hạn 1 request<br>Mặc định =20</td></tr><tr><td>page</td><td>number</td><td></td><td>Số trang<br>Mặc định =1</td></tr><tr><td>keyword</td><td>string</td><td></td><td>Từ khoá tìm kiếm</td></tr></tbody></table>

### Example response

```json

{
    "data": {
        "total": 79,
        "limit": 2,
        "items": [
            {
                "id": "653a06290217d1001230bdee",
                "name": "autochontag",
                "created_at": "2023-10-26T06:24:41.513Z",
                "updated_at": "2023-10-26T06:24:41.513Z"
            },
            {
                "id": "653a052a0217d1001230bb54",
                "name": "tag moi tao tu flow",
                "created_at": "2023-10-26T06:20:26.691Z",
                "updated_at": "2023-10-26T06:20:26.691Z"
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

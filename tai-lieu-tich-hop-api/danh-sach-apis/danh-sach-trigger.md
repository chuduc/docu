# Danh sách Trigger

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/trigger/list](https://api.service.ladiflow.com/1.0/trigger/list)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/trigger/list' \
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

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th><th></th></tr></thead><tbody><tr><td>keyword</td><td>string</td><td></td><td>Từ khóa tìm kiếm</td><td></td></tr><tr><td>page</td><td>Number</td><td></td><td>Số trang<br>Mặc định =1</td><td></td></tr><tr><td>limit</td><td>Number</td><td></td><td>Giới hạn bản ghi/request<br>Mặc định =20</td><td></td></tr></tbody></table>

### Example response

```json
{
    "data": {
        "total": 2,
        "limit": 3,
        "items": [
            {
                "tags": [],
                "_id": "653b2039b5259000120d4675",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "creator_id": "5ebd77abdbd90818b28f8fce",
                "owner_id": "5ebd77abdbd90818b28f8fce",
                "name": "Tags Check PRH MHE",
                "alias": "tags-check-prh-mhe",
                "type": "TAG_APPLY",
                "status": true,
                "flow_id": "653b2037b5259000120d4033",
                "config": {
                    "integration_id": "",
                    "page_id": ""
                },
                "email": {
                    "integration_id": "64ac39ebf43b150013118811"
                },
                "sms": {
                    "integration_id": ""
                },
                "zalo": {
                    "message_template_configs": [],
                    "integration_id": "",
                    "page_id": ""
                },
                "trigger_conditions": [
                    {
                        "condition": {
                            "code": "TAG_APPLIED",
                            "name": "Tag Applied"
                        },
                        "operator": {
                            "code": "EQUAL",
                            "name": "SEGMENTS.OPERATOR_EQUAL"
                        },
                        "value": "651d3edb1038460011673198"
                    }
                ],
                "trigger_operator": "AND",
                "multi_conditions": [],
                "operator": "OR",
                "ref": "ffa454b37d18cd72",
                "all_keyword": false,
                "email_detect": false,
                "phone_detect": false,
                "is_delete": false,
                "hook_mapping_fields": [],
                "created_at": "2023-10-27T02:28:09.574Z",
                "updated_at": "2023-10-27T03:00:18.700Z"
            },
            {
                "tags": [],
                "_id": "653b2039b5259000120d4672",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "creator_id": "5ebd77abdbd90818b28f8fce",
                "owner_id": "5ebd77abdbd90818b28f8fce",
                "name": "Tags vào zoom BHT01",
                "alias": "tags-vao-zoom-bht01",
                "type": "TAG_APPLY",
                "status": true,
                "flow_id": "653b2037b5259000120d4033",
                "config": {
                    "integration_id": "",
                    "page_id": ""
                },
                "email": {
                    "integration_id": "DEFAULT_SES"
                },
                "sms": {
                    "integration_id": ""
                },
                "zalo": {
                    "message_template_configs": [],
                    "integration_id": "",
                    "page_id": ""
                },
                "trigger_conditions": [
                    {
                        "condition": {
                            "code": "TAG_APPLIED",
                            "name": "Tag Applied"
                        },
                        "operator": {
                            "code": "EQUAL",
                            "name": "SEGMENTS.OPERATOR_EQUAL"
                        },
                        "value": "653a46c3b5259000120c31b0"
                    }
                ],
                "trigger_operator": "AND",
                "multi_conditions": [],
                "operator": "OR",
                "ref": "a8b554816cefcba4",
                "all_keyword": false,
                "email_detect": false,
                "phone_detect": false,
                "is_delete": false,
                "hook_mapping_fields": [],
                "created_at": "2023-10-27T02:28:09.560Z",
                "updated_at": "2023-10-27T03:00:18.700Z"
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

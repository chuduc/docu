# Tạo khách hàng

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/customer/create](https://api.service.ladiflow.com/1.0/customer/create)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/customer/create' \
--header 'Api-Key: {{API_KEY}}' \
--data-raw '{
    "email": "test@gmail.com",
    "first_name": "test",
    "full_name": "test",
    "dob": "1989-11-03",
    "phone": null,
    "gender": "male",
    "tags": ["5fffb9c981cf1245fa091985", "5fffb9ce81cf1245fa091986", "5fffb9ce81cf1245fa091900"],
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
    "city": "Hà Nội",
    "address": "68 Nguyễn Cơ Thạch",
    "address_2":"",
    "district": "Nam Từ Liêm",
    "company": "LadiPage",
    "job_title": "Coder",
    "ward": "Mỹ Đình 1",
    "lang": "vi",
    "postal_code": 100000,
    "source": "API",
    "external_customer_id": "123",
    "subcribed_at": "2020-12-01",
    "website": "123",
    "facebook_url": "123",
    "twitter_url": "123",
    "linkedIn_url": "123",
    "score": 14,
    "skype": null,
    "zalo": null
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="156">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="130">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="135">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>email</td><td>string</td><td></td><td>Bắt buộc email hoặc số điện thoại</td></tr><tr><td>first_name</td><td>string</td><td></td><td>Tên</td></tr><tr><td>full_name</td><td>string</td><td></td><td>Họ và tên</td></tr><tr><td>dob</td><td>yyyy-mm-dd</td><td></td><td>Ngày sinh</td></tr><tr><td>phone</td><td>string</td><td></td><td>Số điện thoại<br>Bắt buộc email hoặc số điện thoại</td></tr><tr><td>gender</td><td>male/female</td><td></td><td>Giới tính</td></tr><tr><td>tags</td><td>list</td><td></td><td>Danh sách tag id </td></tr><tr><td>custom_fields</td><td>List Object</td><td></td><td> Các giá trị trường tuỳ chỉnh</td></tr><tr><td>country</td><td>string</td><td></td><td>Quốc gia</td></tr><tr><td>city</td><td>string</td><td></td><td>thành phố</td></tr><tr><td>district</td><td>string</td><td></td><td>Quận huyện</td></tr><tr><td>ward</td><td>string</td><td></td><td>Phường xã</td></tr><tr><td>address</td><td>string</td><td></td><td>Địa chỉ</td></tr><tr><td>company</td><td>string</td><td></td><td>Tên công ty</td></tr><tr><td>job_title</td><td>string</td><td></td><td>Công việc</td></tr><tr><td>lang</td><td>vi/en/other</td><td></td><td>Ngôn ngữ</td></tr><tr><td>postal_code</td><td>number</td><td></td><td>Mã bưu điện</td></tr><tr><td>channels</td><td>list</td><td></td><td>Kênh tương tác</td></tr><tr><td>external_customer_id</td><td>string</td><td></td><td>ID khách hàng từ dữ liệu bên ngoài</td></tr><tr><td>website</td><td>list</td><td></td><td></td></tr><tr><td>facebook_url</td><td>string</td><td></td><td>Đường dẫn tài khoản Facebook</td></tr><tr><td>twitter_url</td><td>string</td><td></td><td>Đường dẫn tài khoản Twitter</td></tr><tr><td>linkedIn_url</td><td>string</td><td></td><td>Đường dẫn tài khoản Linkedln</td></tr><tr><td>score</td><td>number</td><td></td><td>Điểm lead scoring</td></tr><tr><td>zalo</td><td>string</td><td></td><td>Tên zalo</td></tr><tr><td>skype</td><td>string</td><td></td><td>Tên tài khoản Skype</td></tr></tbody></table>

### Example response

```json
{
    "data": {
        "channels": [
            "API"
        ],
        "tags": [],
        "vouchers": [],
        "is_email_verified": false,
        "messenger_recurring_message_tokens": [],
        "messenger_recurring_topics": [],
        "fb_page_ids": [],
        "fb_uids": [],
        "zalo_oa_ids": [],
        "zalo_uids": [],
        "ladichat_uids": [],
        "ladichat_store_ids": [],
        "is_merge": false,
        "is_delete": false,
        "_id": "653a3ca502e8ab00122c39c3",
        "email": "test@gmail.com",
        "key": "test@gmail.com-5f9fa8a09b5c4d6ce6e3a77d",
        "custom_fields": [],
        "name": "test",
        "first_name": "test",
        "last_name": "",
        "gender": "male",
        "dob": "1989-11-03T00:00:00.000Z",
        "dob_year": 1989,
        "dob_month": 10,
        "dob_day": 3,
        "dob_month_day": "1003",
        "company": "LadiPage",
        "job_title": "Coder",
        "city": "Hà Nội",
        "district": "Nam Từ Liêm",
        "address": "68 Nguyễn Cơ Thạch",
        "ward": "Mỹ Đình 1",
        "postal_code": 100000,
        "website": "123",
        "facebook_url": "123",
        "twitter_url": "123",
        "linkedIn_url": "123",
        "alias": "testgmail-com-test",
        "status": "SUBSCRIBER",
        "subscribed_at": "2023-10-26T10:17:09.526Z",
        "external_customer_id": "123",
        "source": "API",
        "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
        "owner_id": "5ebd77abdbd90818b28f8fce",
        "creator_id": "5ebd77abdbd90818b28f8fce",
        "avatar_color": "#0137D3",
        "score": 14,
        "fb_page_uids": [],
        "zalo_oa_uids": [],
        "ladichat_store_uids": [],
        "created_at": "2023-10-26T10:17:09.529Z",
        "updated_at": "2023-10-26T10:17:09.529Z",
        "isNewSubscriber": true,
        "external_data": [
            {
                "name": "full_name",
                "value": "test"
            },
            {
                "name": "lang",
                "value": "vi"
            },
            {
                "name": "subcribed_at",
                "value": "2020-12-01"
            },
            {
                "name": "owner_id",
                "value": "5ebd77abdbd90818b28f8fce"
            },
            {
                "name": "creator_id",
                "value": "5ebd77abdbd90818b28f8fce"
            },
            {
                "name": "is_delete",
                "value": false
            }
        ]
    },
    "message": "Thành công",
    "code": 201
}
```

### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả                       |
| ---------- | ------------ | --------------------------- |
| data       | Object       | Dữ liệu khách hàng được tạo |
| message    | string       | Thông điệp                  |
| code       | number       | Mã phản hồi                 |

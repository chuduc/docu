# Chi tiết khách hàng

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/customer/](https://api.service.ladiflow.com/1.0/customer/create)[show](https://api.service.ladiflow.com/1.0/customer/show)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/customer/show' \
--header 'Api-Key: {API-KEY}' \
--header 'Content-Type: application/json' \
--data-raw '{
    "customer_id": "662c801d7fd0573d9b2f23a8",
    "email":"0363042200.ladiflow@ladimail.com",
    "phone": "0363042200"
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="118">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="158">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>customer_id</td><td>string</td><td></td><td>id khách hàng<br>Bắt buộc 1 trong 3 dữ liệu customer_id, email, phone</td></tr><tr><td>email</td><td>string</td><td></td><td>Email khách hàng muốn tìm<br>Bắt buộc 1 trong 3 dữ liệu customer_id, email, phone</td></tr><tr><td>phone</td><td>string</td><td></td><td>Số điện thoại<br>Bắt buộc 1 trong 3 dữ liệu customer_id, email, phone</td></tr></tbody></table>

### Example response

```json
{
    "data": {
        "customer": {
            "channels": [
                "NHANHVN",
                "DASHBOARD",
                "ZALO"
            ],
            "tags": [
                "65b35536a145a5001292ac32",
                "662235cb9b219f00123b6289"
            ],
            "vouchers": [
                "S24CNXRIW4",
                "LDFG0K7_OEY",
                "LDFGXSOY79S"
            ],
            "is_email_verified": false,
            "messenger_recurring_message_tokens": [],
            "messenger_recurring_topics": [],
            "fb_page_ids": [],
            "fb_uids": [],
            "zalo_oa_ids": [
                "3657925253147481196"
            ],
            "zalo_uids": [
                "8870236147300259240"
            ],
            "ladichat_uids": [],
            "ladichat_store_ids": [],
            "is_merge": true,
            "is_delete": false,
            "_id": "662c801d7fd0573d9b2f23a8",
            "email": "0363042200.ladiflow@ladimail.com",
            "key": "0363042200.ladiflow@ladimail.com-5f9fa8a09b5c4d6ce6e3a77d",
            "custom_fields": [
                {
                    "values": [],
                    "name": "last_order_discount_total",
                    "value": 0,
                    "data_type": "NUMBER"
                },
                {
                    "values": [],
                    "name": "last_order_shipping_fee",
                    "value": "",
                    "data_type": "NUMBER"
                },
                {
                    "values": [],
                    "name": "order_total",
                    "value": 0,
                    "data_type": "NUMBER"
                },
                {
                    "values": [],
                    "name": "payment_method",
                    "value": "2"
                },
                {
                    "values": [
                        "173672",
                        null
                    ],
                    "custom_field_id": "61e0dbf1e5f4c20013f4a23c",
                    "name": "channel_urls",
                    "data_type": "CHECK_BOX"
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b35645c011a0b4c70e",
                    "name": "last_order_id",
                    "data_type": "TEXT_INPUT",
                    "value": "2"
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b35645c011a0b4c70f",
                    "name": "last_order_code",
                    "data_type": "TEXT_INPUT",
                    "value": "2"
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b35645c011a0b4c710",
                    "name": "last_order_status",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b35645c011a0b4c711",
                    "name": "last_order_total",
                    "data_type": "NUMBER",
                    "value": 321321
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c721",
                    "name": "last_order_discount_note",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c722",
                    "name": "last_order_discount_code",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c724",
                    "name": "last_order_shipping_status",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c725",
                    "name": "last_order_shipping_address",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c726",
                    "name": "last_order_payment_method",
                    "data_type": "TEXT_INPUT",
                    "value": "2"
                },
                {
                    "values": [],
                    "custom_field_id": "626a54b45645c011a0b4c727",
                    "name": "last_order_payment_status",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                },
                {
                    "values": [],
                    "custom_field_id": "627dc60744411b00152e9541",
                    "name": "last_order_created_at",
                    "data_type": "DATE",
                    "value": "2024-04-25T07:02:50.000Z"
                },
                {
                    "values": [],
                    "custom_field_id": "627dc60744411b00152e9544",
                    "name": "last_order_updated_at",
                    "data_type": "DATE",
                    "value": "2024-04-25T07:02:50.000Z"
                },
                {
                    "values": [],
                    "custom_field_id": "628211f13534ff3f689c1836",
                    "name": "last_order_product_names",
                    "data_type": "LIST"
                },
                {
                    "values": [],
                    "custom_field_id": "628211f13534ff3f689c1837",
                    "name": "last_order_product_ids",
                    "data_type": "LIST"
                },
                {
                    "values": [],
                    "custom_field_id": "628211f13534ff3f689c1838",
                    "name": "last_order_product_skus",
                    "data_type": "LIST"
                },
                {
                    "values": [],
                    "custom_field_id": "6433d76f1557c942c0e4979b",
                    "name": "last_order_tracking_code",
                    "data_type": "TEXT_INPUT",
                    "value": ""
                }
            ],
            "last_name": "",
            "phone": "0363042200",
            "gender": "female",
            "dob": "2024-04-10T00:00:00.000Z",
            "dob_year": 2024,
            "dob_month": 3,
            "dob_day": 10,
            "dob_month_day": "0310",
            "company": "qwewqewq",
            "country": "Việt Nam",
            "country_id": "VN",
            "address": "Hn",
            "alias": "0363042200-ladiflowladimail-com-nguyen-manh-dung-nguyen-manh-dung-0363042200-qwewqewq",
            "status": "SUBSCRIBER",
            "subscribed_at": "2024-04-27T04:33:33.445Z",
            "external_customer_id": "1",
            "source": "ZALO",
            "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
            "avatar_color": "#E1A046",
            "score": 0,
            "fb_page_uids": [],
            "zalo_oa_uids": [
                {
                    "zalo_oa_id": "3657925253147481196",
                    "zalo_uid": "8870236147300259240",
                    "primary": true
                }
            ],
            "ladichat_store_uids": [],
            "created_at": "2024-04-27T04:33:33.462Z",
            "updated_at": "2024-05-16T04:10:05.614Z",
            "first_name": "Nguyễn Mạnh Dũng",
            "name": "Nguyễn Mạnh Dũng",
            "last_voucher_code": "LDFG0K7_OEY",
            "address_2": null,
            "city": null,
            "city_id": null,
            "creator_id": "5ebd77abdbd90818b28f8fce",
            "district": null,
            "district_id": null,
            "language": "vi",
            "owner_id": "5ebd77abdbd90818b28f8fce",
            "phone_2": null,
            "postal_code": null,
            "ward": null,
            "ward_id": null,
            "avatar": "https://s120-ava-talk.zadn.vn/a/c/2/7/4/120/0b402e431b681dafda3520970dc4ea0f.jpg",
            "zalo_uid_by_app": "9155380902899175694",
            "bounce": 0,
            "complaint": 0,
            "email_subscribe_status": true,
            "avg_cancel_order_value": 0,
            "avg_order_value": 0,
            "avg_paid_order_value": 0,
            "avg_pending_order_value": 0,
            "facebook_url": null,
            "ipos_membership_id": null,
            "job_title": null,
            "linkedIn_url": null,
            "skype": null,
            "total_cancel_order": 0,
            "total_cancel_order_value": 0,
            "total_order": 0,
            "total_order_value": 0,
            "total_paid_order": 0,
            "total_paid_order_value": 0,
            "total_pending_order": 0,
            "total_pending_order_value": 0,
            "twitter_url": null,
            "website": null,
            "zalo": null
        }
    },
    "message": "Thành công",
    "code": 200
}
```

### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả               |
| ---------- | ------------ | ------------------- |
| data       | Object       | Dữ liệu khách hàng  |
| message    | Object       | Thông điệp          |
| code       | Number       | Mã phản hồi         |

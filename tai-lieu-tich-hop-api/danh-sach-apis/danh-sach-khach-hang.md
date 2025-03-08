# Danh sách khách hàng

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/customer/list](https://api.service.ladiflow.com/1.0/customer/list)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```
curl --location 'https://api.service.ladiflow.com/1.0/customer/list' \
--header 'api-key: 8ad68ed712beab4631e0882036d7e6381b67870edb280c4d' \
--header 'Content-Type: application/json' \
--data-raw '{
    "search": {
        "name": "dungnguyen.ladipage@gmail.com"  
    },
    "page": 1,
    "limit": 10,
    "sort": {
        "updated_at": "DESC"
    },
    "tags": [] 
}'
```

### &#x20;Tham số header

<table><thead><tr><th width="155">Tham số</th><th width="127">Kiểu dữ liệu</th><th width="163">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Api-Key</td><td>string</td><td>có</td><td>API key lấy trên LadiFlow</td></tr></tbody></table>

### Tham số Body

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="165">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>name</td><td>string</td><td></td><td>Tìm kiếm theo tên, email hoặc số điện thoai của khách hàng</td></tr><tr><td>tags</td><td>list</td><td></td><td>Danh sách tag id </td></tr></tbody></table>

### Example response

```
{
    "data": {
        "total": 1,
        "limit": 10,
        "items": [
            {
                "score": 5,
                "channels": [
                    "DASHBOARD"
                ],
                "tags": [
                    "66b1c29c72b9ba001265138a"
                ],
                "vouchers": [],
                "is_email_verified": true,
                "email_subscribe_status": true,
                "bounce": 0,
                "complaint": 0,
                "total_order": 0,
                "total_order_value": 0,
                "avg_order_value": 0,
                "total_pending_order": 0,
                "total_pending_order_value": 0,
                "avg_pending_order_value": 0,
                "total_paid_order": 0,
                "total_paid_order_value": 0,
                "avg_paid_order_value": 0,
                "total_cancel_order": 0,
                "total_cancel_order_value": 0,
                "avg_cancel_order_value": 0,
                "messenger_recurring_message_tokens": [],
                "messenger_recurring_topics": [],
                "fb_page_ids": [],
                "fb_uids": [],
                "zalo_oa_ids": [],
                "zalo_uids": [],
                "ladichat_uids": [],
                "ladichat_store_ids": [],
                "is_merge": false,
                "phone_verified": false,
                "is_delete": false,
                "email": "dungnguyen.ladipage@gmail.com",
                "key": "dungnguyen.ladipage@gmail.com-5f9fa8a09b5c4d6ce6e3a77d",
                "custom_fields": [
                    {
                        "custom_field_id": "658cde870f578500124e6f87",
                        "name": "point",
                        "data_type": "NUMBER",
                        "value_number": 0,
                        "order": 0
                    },
                    {
                        "values": [
                            "null"
                        ],
                        "custom_field_id": "61e0dbf1e5f4c20013f4a23c",
                        "name": "channel_urls",
                        "data_type": "CHECK_BOX",
                        "order": 1
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b35645c011a0b4c70e",
                        "name": "last_order_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 2
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b35645c011a0b4c70f",
                        "name": "last_order_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 3
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b35645c011a0b4c710",
                        "name": "last_order_status",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 4
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c721",
                        "name": "last_order_discount_note",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 5
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c722",
                        "name": "last_order_discount_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 6
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c724",
                        "name": "last_order_shipping_status",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 7
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c725",
                        "name": "last_order_shipping_address",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 8
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c726",
                        "name": "last_order_payment_method",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 9
                    },
                    {
                        "values": [],
                        "custom_field_id": "626a54b45645c011a0b4c727",
                        "name": "last_order_payment_status",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 10
                    },
                    {
                        "values": [],
                        "custom_field_id": "627dc60744411b00152e9541",
                        "name": "last_order_created_at",
                        "data_type": "DATE",
                        "value": "",
                        "order": 11
                    },
                    {
                        "values": [],
                        "custom_field_id": "627dc60744411b00152e9544",
                        "name": "last_order_updated_at",
                        "data_type": "DATE",
                        "value": "",
                        "order": 12
                    },
                    {
                        "values": [],
                        "custom_field_id": "628211f13534ff3f689c1836",
                        "name": "last_order_product_names",
                        "data_type": "LIST",
                        "order": 13
                    },
                    {
                        "values": [],
                        "custom_field_id": "628211f13534ff3f689c1837",
                        "name": "last_order_product_ids",
                        "data_type": "LIST",
                        "order": 14
                    },
                    {
                        "values": [],
                        "custom_field_id": "628211f13534ff3f689c1838",
                        "name": "last_order_product_skus",
                        "data_type": "LIST",
                        "order": 15
                    },
                    {
                        "values": [],
                        "custom_field_id": "6433d76f1557c942c0e4979b",
                        "name": "last_order_tracking_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 16
                    },
                    {
                        "values": [],
                        "custom_field_id": "64423cf353f041324448933d",
                        "name": "text",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 17
                    },
                    {
                        "values": [],
                        "custom_field_id": "64423d0753f041324448933e",
                        "name": "doan_text",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 18
                    },
                    {
                        "values": [],
                        "custom_field_id": "64474003121e5600129cb22d",
                        "name": "list_list",
                        "data_type": "LIST",
                        "order": 19
                    },
                    {
                        "values": [],
                        "custom_field_id": "645356d344a0584730243ea1",
                        "name": "boolean",
                        "data_type": "BOOLEAN",
                        "value": "",
                        "order": 20
                    },
                    {
                        "values": [],
                        "custom_field_id": "652cdcf0a816b300124502d8",
                        "name": "join_supported_group_status",
                        "data_type": "BOOLEAN",
                        "value": "",
                        "order": 21
                    },
                    {
                        "values": [],
                        "custom_field_id": "6538888eeedd2a0012158326",
                        "name": "course_list",
                        "data_type": "LIST",
                        "order": 22
                    },
                    {
                        "values": [],
                        "custom_field_id": "653888a5eedd2a00121583e5",
                        "name": "course_register_date_list",
                        "data_type": "LIST",
                        "order": 23
                    },
                    {
                        "values": [],
                        "custom_field_id": "65682ee7aa075b0012035d8c",
                        "name": "ldptext",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 24
                    },
                    {
                        "values": [],
                        "custom_field_id": "65682f17aa075b0012035e53",
                        "name": "ldprb",
                        "data_type": "DROPDOWN",
                        "order": 25
                    },
                    {
                        "values": [],
                        "custom_field_id": "65682f2aaa075b0012035e68",
                        "name": "ldpcheckbox",
                        "data_type": "CHECK_BOX",
                        "order": 26
                    },
                    {
                        "values": [],
                        "custom_field_id": "65694544aa075b0012060ca2",
                        "name": "checkbox_test",
                        "data_type": "CHECK_BOX",
                        "order": 27
                    },
                    {
                        "values": [],
                        "custom_field_id": "656ffa981d251d00126c19ef",
                        "name": "boolean_field",
                        "data_type": "BOOLEAN",
                        "value": "",
                        "order": 28
                    },
                    {
                        "values": [],
                        "custom_field_id": "658a86e424caf200129ca6fb",
                        "name": "voucher_campaign_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 29
                    },
                    {
                        "values": [],
                        "custom_field_id": "658cdd7c0f578500124e696b",
                        "name": "last_voucher_date_start",
                        "data_type": "DATE",
                        "value": "",
                        "order": 30
                    },
                    {
                        "values": [],
                        "custom_field_id": "658cdda50f578500124e6c02",
                        "name": "last_voucher_date_end",
                        "data_type": "DATE",
                        "value": "",
                        "order": 31
                    },
                    {
                        "values": [],
                        "custom_field_id": "658e83ff0f578500125488c0",
                        "name": "last_vouher_campaign_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 32
                    },
                    {
                        "values": [],
                        "custom_field_id": "658e84110f578500125488d3",
                        "name": "last_voucher_campaign_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 33
                    },
                    {
                        "values": [],
                        "custom_field_id": "6595203d3cf3970012b17762",
                        "name": "last_voucher_campaign_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 34
                    },
                    {
                        "values": [],
                        "custom_field_id": "65aa25e06e18890013f2b988",
                        "name": "note",
                        "data_type": "TEXT_INPUT",
                        "value": "tăng điểm",
                        "order": 35
                    },
                    {
                        "values": [],
                        "custom_field_id": "65b879d3c7769000121aba57",
                        "name": "last_survey_submit",
                        "data_type": "DATE",
                        "value": "",
                        "order": 36
                    },
                    {
                        "values": [],
                        "custom_field_id": "65b879f0c7769000121abb5f",
                        "name": "last_survey_feedback",
                        "data_type": "LIST",
                        "order": 37
                    },
                    {
                        "values": [],
                        "custom_field_id": "65b87a07c7769000121abd35",
                        "name": "last_survey_note",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 38
                    },
                    {
                        "values": [],
                        "custom_field_id": "65fd2629a0897c00124ab7d7",
                        "name": "tudongtang",
                        "data_type": "AUTO_INCREMENT",
                        "value": "",
                        "order": 39
                    },
                    {
                        "values": [],
                        "custom_field_id": "6600e684a0897c0012518254",
                        "name": "assign",
                        "data_type": "DATE",
                        "value": "",
                        "order": 40
                    },
                    {
                        "values": [],
                        "custom_field_id": "660cba6222796c001213ef6d",
                        "name": "otp_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 41
                    },
                    {
                        "values": [],
                        "custom_field_id": "660ce14222796c00121527b0",
                        "name": "ldp_test",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 42
                    },
                    {
                        "values": [],
                        "custom_field_id": "6610b64813bc320013c1c6b4",
                        "name": "package_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 43
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614a0802437680013310ef3",
                        "name": "is_tag",
                        "data_type": "BOOLEAN",
                        "value": "",
                        "order": 44
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7a292b9220012af71ec",
                        "name": "lds_event_ticket_seat_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 45
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7b192b9220012af728e",
                        "name": "lds_event_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 46
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7c092b9220012af72f6",
                        "name": "lds_event_ticket_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 47
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7cf92b9220012af737d",
                        "name": "lds_event_checked_in_time",
                        "data_type": "DATE",
                        "value": "",
                        "order": 48
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7e092b9220012af749a",
                        "name": "lds_event_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 49
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b7f492b9220012af7575",
                        "name": "lds_event_ticket_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 50
                    },
                    {
                        "values": [],
                        "custom_field_id": "6614b80192b9220012af765d",
                        "name": "lds_event_ticket_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 51
                    },
                    {
                        "values": [],
                        "custom_field_id": "6615f7775730f60012ddd348",
                        "name": "danhxung",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 52
                    },
                    {
                        "values": [],
                        "custom_field_id": "661cfd84d9233500131b0f09",
                        "name": "membership_type_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 53
                    },
                    {
                        "values": [],
                        "custom_field_id": "661dee0ed9233500131d5740",
                        "name": "end_date",
                        "data_type": "DATE",
                        "value": "",
                        "order": 54
                    },
                    {
                        "values": [],
                        "custom_field_id": "661def3cd9233500131d6ea8",
                        "name": "coupon_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 55
                    },
                    {
                        "values": [],
                        "custom_field_id": "661e3be6ba63b900127eb526",
                        "name": "ngaynao",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 56
                    },
                    {
                        "values": [],
                        "custom_field_id": "66262467676fb20012eb8ad4",
                        "name": "ldf_voucher_remind_expire_date",
                        "data_type": "DATE",
                        "value": "",
                        "order": 57
                    },
                    {
                        "values": [],
                        "custom_field_id": "662a15b4fb21de0012aa37e4",
                        "name": "nhanhvn_code",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 58
                    },
                    {
                        "values": [],
                        "custom_field_id": "662a15c0fb21de0012aa38cf",
                        "name": "nhanhvn_level",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 59
                    },
                    {
                        "values": [],
                        "custom_field_id": "662a15c9fb21de0012aa38ed",
                        "name": "nhanhvn_group",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 60
                    },
                    {
                        "values": [],
                        "custom_field_id": "662a15ddfb21de0012aa3988",
                        "name": "first_order_created_date",
                        "data_type": "DATE",
                        "value": "",
                        "order": 61
                    },
                    {
                        "values": [],
                        "custom_field_id": "66334d964c4e970012a42c0f",
                        "name": "last_order_created_date",
                        "data_type": "DATE",
                        "value": "",
                        "order": 62
                    },
                    {
                        "values": [],
                        "custom_field_id": "66334dae4c4e970012a42c37",
                        "name": "last_order_mode",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 63
                    },
                    {
                        "values": [],
                        "custom_field_id": "66334dc84c4e970012a42c88",
                        "name": "nhanh_last_sale_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 64
                    },
                    {
                        "values": [],
                        "custom_field_id": "66334dd54c4e970012a42cc6",
                        "name": "last_order_created_by_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 65
                    },
                    {
                        "values": [],
                        "custom_field_id": "66458561981b190012146c3d",
                        "name": "doncuoi",
                        "data_type": "CHECK_BOX",
                        "order": 66
                    },
                    {
                        "values": [],
                        "custom_field_id": "6646d158b7321300121a0185",
                        "name": "last_order_date",
                        "data_type": "DATE",
                        "value": "",
                        "order": 67
                    },
                    {
                        "values": [],
                        "custom_field_id": "6646d166b7321300121a0205",
                        "name": "nhanhvn_first_depot_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 68
                    },
                    {
                        "values": [],
                        "custom_field_id": "6646d173b7321300121a0247",
                        "name": "nhanhvn_first_depot_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 69
                    },
                    {
                        "values": [],
                        "custom_field_id": "6646d182b7321300121a028e",
                        "name": "nhanhvn_last_depot_name",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 70
                    },
                    {
                        "values": [],
                        "custom_field_id": "6646d18bb7321300121a0295",
                        "name": "nhanhvn_last_depot_id",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 71
                    },
                    {
                        "values": [],
                        "custom_field_id": "664ea1e2e4efe40012502c54",
                        "name": "solanmua",
                        "data_type": "AUTO_INCREMENT",
                        "value": "",
                        "order": 72
                    },
                    {
                        "values": [],
                        "custom_field_id": "664ea94a952c6900122cd1ce",
                        "name": "songaymua",
                        "data_type": "AUTO_INCREMENT",
                        "value": "",
                        "order": 73
                    },
                    {
                        "values": [],
                        "custom_field_id": "6656a5b19bddeb0013ea9220",
                        "name": "ttinzzzz",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 74
                    },
                    {
                        "values": [],
                        "custom_field_id": "6656a5e09bddeb0013ea9495",
                        "name": "ttin1212",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 75
                    },
                    {
                        "values": [],
                        "custom_field_id": "6656b05b9bddeb0013eb8e8f",
                        "name": "boooossadw",
                        "data_type": "BOOLEAN",
                        "value": "",
                        "order": 76
                    },
                    {
                        "values": [],
                        "custom_field_id": "666270afc90d0d0012b4f85b",
                        "name": "click_link_sms_ads",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 77
                    },
                    {
                        "values": [],
                        "custom_field_id": "66627a90c90d0d0012b549bf",
                        "name": "ldp_team",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 78
                    },
                    {
                        "values": [],
                        "custom_field_id": "666ba66b9bf783001386eeb7",
                        "name": "this_field_is_new",
                        "data_type": "DATE",
                        "value": "",
                        "order": 79
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c05f4b34989001249a981",
                        "name": "dcnhan",
                        "data_type": "TEXT_AREA",
                        "value": "",
                        "order": 80
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c060cb34989001249a98a",
                        "name": "dctt",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 81
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c061bb34989001249a991",
                        "name": "socccd",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 82
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c0637b34989001249a99c",
                        "name": "ngaycapcccd",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 83
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c0643b34989001249a9a3",
                        "name": "vanbang",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 84
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c0653b34989001249a9aa",
                        "name": "sochungchi",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 85
                    },
                    {
                        "values": [],
                        "custom_field_id": "667c0664b34989001249a9b3",
                        "name": "ngaycap2",
                        "data_type": "DATE",
                        "value": "",
                        "order": 86
                    },
                    {
                        "values": [],
                        "custom_field_id": "66820624a317f82070596ada",
                        "name": "Ten_Truong_Dai_Hoc",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 87
                    },
                    {
                        "values": [],
                        "custom_field_id": "6682083c87eff00012aa9c51",
                        "name": "test_ldf",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 88
                    },
                    {
                        "values": [],
                        "custom_field_id": "66825117ce5ef90012de1b4d",
                        "name": "dat_test",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 89
                    },
                    {
                        "values": [],
                        "custom_field_id": "66852b37bf7e2e00123b4a59",
                        "name": "dang_list",
                        "data_type": "LIST",
                        "order": 90
                    },
                    {
                        "values": [],
                        "custom_field_id": "668f3f0cddc8fb0012685847",
                        "name": "qr_list",
                        "data_type": "LIST",
                        "order": 91
                    },
                    {
                        "values": [],
                        "custom_field_id": "668f9eadc29364001227e07d",
                        "name": "qr_hop_chon",
                        "data_type": "DROPDOWN",
                        "order": 92
                    },
                    {
                        "values": [],
                        "custom_field_id": "6690a719f0010f00124e3df7",
                        "name": "lds_qr_code_url",
                        "data_type": "LIST",
                        "order": 93
                    },
                    {
                        "values": [],
                        "custom_field_id": "6690ab5ff0010f00124e5993",
                        "name": "new_fielddd",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 94
                    },
                    {
                        "values": [],
                        "custom_field_id": "6690d1056f95320013f0ca5b",
                        "name": "qr_hop_kiem",
                        "data_type": "CHECK_BOX",
                        "order": 95
                    },
                    {
                        "values": [],
                        "custom_field_id": "6695e967d6b02800120bf997",
                        "name": "lds_last_qr_code_urls",
                        "data_type": "LIST",
                        "order": 96
                    },
                    {
                        "values": [],
                        "custom_field_id": "66a766ed91df320012731f5f",
                        "name": "voucher_remaining_days_1",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 97
                    },
                    {
                        "values": [],
                        "custom_field_id": "66a7684f91df3200127324d9",
                        "name": "custom_field_a",
                        "data_type": "TEXT_INPUT",
                        "value": "",
                        "order": 98
                    },
                    {
                        "custom_field_id": "66b197b102941300120b1798",
                        "name": "order_number",
                        "data_type": "NUMBER",
                        "oldValue": null,
                        "newValues": [],
                        "value_number": "12",
                        "order": 99
                    }
                ],
                "name": "dung",
                "first_name": "dung",
                "last_name": "",
                "phone": "0363042200",
                "gender": "male",
                "dob": "1970-01-01T00:00:00.000Z",
                "dob_year": 1970,
                "dob_month": 0,
                "dob_day": 1,
                "dob_month_day": "0001",
                "language": "vi",
                "alias": "dungnguyen-ladipagegmail-com-dung-0363042200",
                "status": "SUBSCRIBER",
                "subscribed_at": "2024-07-27T02:52:11.341Z",
                "source": "DASHBOARD",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "owner_id": "5ebd77abdbd90818b28f8fce",
                "creator_id": "5ebd77abdbd90818b28f8fce",
                "avatar_color": "#C3413F",
                "source_customer": "",
                "fb_page_uids": [],
                "zalo_oa_uids": [],
                "ladichat_store_uids": [],
                "created_at": "2024-07-29T07:48:42.988Z",
                "updated_at": "2024-08-10T09:22:06.413Z",
                "id": "66a7495ab6c13a6af92a80cf",
                "postal_code": null,
                "country": null,
                "address_2": null,
                "phone_2": null,
                "district": null,
                "country_id": null,
                "ward_id": null,
                "city_id": null,
                "city": null,
                "ward": null,
                "address": null,
                "district_id": null,
                "_id": "66a7495ab6c13a6af92a80cf"
            }
        ],
        "total_verified": 1
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

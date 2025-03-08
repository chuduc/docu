# Xem chi tiết giao dịch của Flow/Campaign/Sequence

### HTTP request

* API: [https://api.service.ladiflow.com/1.0/](https://api.service.ladiflow.com/1.0/sequence/subscribe)[flow/list-transaction](https://api.service.ladiflow.com/1.0/flow/list-transaction)
* Method: POST
* Content type: application/json
* Response type: Text/json

### Example Request

```jsdoc
curl --location 'https://api.service.ladiflow.com/1.0/flow/list-transaction' \
--header 'Api-Key: {API-KEY}' \
--header 'Content-Type: application/json' \
--data '{
    "from_date": "2024-04-18T17:00:00.610Z",
    "to_date": null,
    "page": 1,
    "limit": 10,
    "sort": {
        "UPDATED_AT": "DESC"
    },
     "type": null,
     "source": null,
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

<table><thead><tr><th width="154">Tham số</th><th width="124">Kiểu dữ liệu</th><th width="125">Bắt buộc</th><th width="374">Mô tả</th></tr></thead><tbody><tr><td>from_date</td><td>string</td><td>Có</td><td>Thời gian bắt đầu lấy dữ liệu</td></tr><tr><td>to_date</td><td>string</td><td>Không</td><td>Thời gian kết thúc lấy dữ liệu</td></tr><tr><td>type</td><td>string</td><td>Không</td><td>Mã hành động muốn xem chi phí. Xem danh sách mã hành động tại <a data-mention href="./#danh-sach-ma-hanh-dong-cua-flow-campaign-sequence">#danh-sach-ma-hanh-dong-cua-flow-campaign-sequence</a></td></tr><tr><td>page</td><td>number</td><td>có</td><td>Số trang muốn lấy dữ liệu. Mặc định =1</td></tr><tr><td>limit</td><td>number</td><td>có</td><td>Số bản ghi tối đa 1 trang, mặc định =10</td></tr><tr><td>sort</td><td>object</td><td>không</td><td>Sắp xếp bản ghi theo điều kiện. Điều kiện có dạng: "tên trường":"loại sắp xếp"<br>Mặc định sắp xếp theo thời gian cập nhật mới nhất</td></tr><tr><td>source</td><td>string</td><td>Có</td><td>Loại chiến dịch: <br>- FLOW<br>- CAMPAIGN<br>- SEQUENCE<br>Phải có giá trị ID chiến dịch tương ứng. Ví dụ source= FLOW thì flow_id bắt buộc</td></tr><tr><td>flow_id</td><td>string</td><td>Không</td><td>ID của Flow</td></tr><tr><td>trigger_id</td><td>string</td><td>Không</td><td>ID của trigger trong flow</td></tr><tr><td>flow_config_id</td><td>string</td><td>Không</td><td>ID của hành động trong flow</td></tr><tr><td>campaign_id</td><td>string</td><td>Không</td><td>ID của Campaign</td></tr><tr><td>sequence_id</td><td>string</td><td>Không</td><td>ID của Sequence</td></tr></tbody></table>

#### Example response

```json
{
    "data": {
        "total": 1642,
        "limit": 10,
        "items": [
            {
                "_id": "66487773577fe90012dc9a4c",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "65b77a4d9970e3001274d148",
                "app_trans_id": "411b7c98-be38-45ce-bf3f-3f3f1e097eaa",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 2,
                "note": null,
                "status": "DONE",
                "type": "EMAIL",
                "trigger_id": "66487743d8d9450012130c04",
                "flow_id": "66487746d8d9450012130c7a",
                "flow_config_id": "66487746d8d9450012130c7c",
                "customer_id": "6614a1d33d83f379673b5e49",
                "trigger_type": "BROADCAST",
                "created_at": "2024-05-18T09:40:03.179Z",
                "updated_at": "2024-05-18T09:40:10.058Z"
            },
            {
                "_id": "66486dd6577fe90012da4252",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "66271afb676fb20012ed4438",
                "app_trans_id": "4661cdcf-2509-4842-ab14-a83a352b52d7",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ZALO_CARE",
                "trigger_id": "66486508d8d9450012127bf9",
                "flow_id": "66486500d8d9450012127af1",
                "flow_config_id": "66486528d8d9450012127d8e",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:59:02.306Z",
                "updated_at": "2024-05-18T08:59:10.054Z"
            },
            {
                "_id": "66486ce6577fe90012da2efe",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "66271afb676fb20012ed4438",
                "app_trans_id": "196cd324-80b7-491f-b96f-326d3c971221",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ZALO_CARE",
                "trigger_id": "66486c88d8d945001212e58f",
                "flow_id": "66486500d8d9450012127af1",
                "flow_config_id": "66486528d8d9450012127d8e",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:55:02.376Z",
                "updated_at": "2024-05-18T08:55:10.064Z"
            },
            {
                "_id": "664864b2577fe90012d98494",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "66271afb676fb20012ed4438",
                "app_trans_id": "00bef8af-5ebf-4488-a360-b9bbf2ac7d18",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ZALO_CARE",
                "trigger_id": "664859e5d8d9450012120aae",
                "flow_id": "66484c3dd8d9450012118785",
                "flow_config_id": "66485713d8d945001211d215",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:20:02.392Z",
                "updated_at": "2024-05-18T08:20:10.089Z"
            },
            {
                "_id": "6648630e577fe90012d95fa7",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "66271afb676fb20012ed4438",
                "app_trans_id": "04343355-3425-476d-9ef7-43e517d5181f",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ZALO_CARE",
                "trigger_id": "66485939d8d945001211f14f",
                "flow_id": "66484c3dd8d9450012118785",
                "flow_config_id": "66485713d8d945001211d215",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:13:02.393Z",
                "updated_at": "2024-05-18T08:13:10.059Z"
            },
            {
                "_id": "6648616b577fe90012d92eb9",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": "66271afb676fb20012ed4438",
                "app_trans_id": "626985b4-c35f-4740-b51f-ced67e2f2893",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ZALO_CARE",
                "trigger_id": "66485939d8d945001211f14f",
                "flow_id": "66484c3dd8d9450012118785",
                "flow_config_id": "66485713d8d945001211d215",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:06:03.565Z",
                "updated_at": "2024-05-18T08:06:10.098Z"
            },
            {
                "_id": "6648616a577fe90012d92e8e",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": null,
                "app_trans_id": "83bf0dc1-fcd8-463c-869a-9414ba883d41",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ADD_TAG",
                "trigger_id": "66485939d8d945001211f14f",
                "flow_id": "66484c3dd8d9450012118785",
                "flow_config_id": "66485363d8d945001211b13b",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:06:02.336Z",
                "updated_at": "2024-05-18T08:06:10.098Z"
            },
            {
                "_id": "66486133577fe90012d927c0",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": null,
                "app_trans_id": "7d9fcd90-c4c0-43e7-aab4-ed6ebefbf85c",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "ADD_VOUCHER",
                "trigger_id": "66486104d8d9450012125568",
                "flow_id": "66486101d8d9450012125478",
                "flow_config_id": "6648610cd8d9450012125660",
                "customer_id": "6644697c733f5a0012114382",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T08:05:07.792Z",
                "updated_at": "2024-05-18T08:05:10.082Z"
            },
            {
                "_id": "664858de2524fb001259d0c7",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": null,
                "app_trans_id": "b658578d-cd05-4ffe-a3d8-d5c48500a72d",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "SENT_NOTIFICATION",
                "trigger_id": "663ce59058b6c70012665e57",
                "flow_id": "663ce59058b6c70012665e37",
                "flow_config_id": "663ce59058b6c70012665e43",
                "customer_id": "65b870b743c884001248a314",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T07:29:34.032Z",
                "updated_at": "2024-05-18T07:29:40.077Z"
            },
            {
                "_id": "664858de577fe90012d62848",
                "store_id": "5f9fa8a09b5c4d6ce6e3a77d",
                "integration_id": null,
                "app_trans_id": "f706122f-bf28-40f4-8f3d-5d65ac8c28aa",
                "ladi_uid": "5ebd77abdbd90818b28f8fce",
                "money": 0,
                "credits": 1,
                "note": null,
                "status": "DONE",
                "type": "CONDITION",
                "trigger_id": "663ce59058b6c70012665e57",
                "flow_id": "663ce59058b6c70012665e37",
                "flow_config_id": "663ce59058b6c70012665e3e",
                "customer_id": "65b870b743c884001248a314",
                "trigger_type": "TRIGGER",
                "created_at": "2024-05-18T07:29:34.043Z",
                "updated_at": "2024-05-18T07:29:40.077Z"
            }
        ]
    },
    "message": "Thành công",
    "code": 200
}
```

#### Cấu trúc thuộc tính data <a href="#cau-truc-thuoc-tinh-data" id="cau-truc-thuoc-tinh-data"></a>

| Thuộc tính | Kiểu dữ liệu | Mô tả                   |
| ---------- | ------------ | ----------------------- |
| data       | Object       | Danh sách các giao dịch |
| message    | string       | Thông điệp              |
| code       | number       | Mã phản hồi             |

# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get info của UID</summary>


```http
GET http://graph.scanfb.top/graph/{UID}/?access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `{UID}` | `string` | **Bắc buộc**. UID cần check thông tin  |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
    "success": true,
    "message": "",
    "data": {
        "id": "100025113282190",
        "about": "Not thing to see",
        "education": [
            {
                "school": {
                    "id": "110057887024664",
                    "name": "Trường Đại học Bách khoa - ĐH Quốc gia TP.HCM"
                },
                "type": "College",
                "id": "1347757829404647"
            },
            {
                "school": {
                    "id": "1450466505186978",
                    "name": "THPT Phước Bình"
                },
                "type": "High School",
                "id": "502456701109337"
            }
        ],
        "first_name": "AnhKiệt",
        "gender": "male",
        "hometown": {
            "id": "109916112357708",
            "name": "Binh Phuoc, Vietnam"
        },
        "last_name": "Nguyễn",
        "link": "https://www.facebook.com/anhkiet9052",
        "location": {
            "id": "108458769184495",
            "name": "Thành phố Hồ Chí Minh"
        },
        "locale": "vi_VN",
        "name": "Nguyễn AnhKiệt",
        "relationship_status": "Hẹn hò",
        "significant_other": {
            "name": "Phương Thảo",
            "id": "100017141862138"
        },
        "timezone": 7,
        "updated_time": "2024-03-15T01:13:27+07:00",
        "username": "anhkiet9052",
        "work": [
            {
                "end_date": "0000-00",
                "employer": {
                    "id": "114740914829344",
                    "name": "Kingcontent.pro"
                },
                "position": {
                    "id": "1561201824136247",
                    "name": ".NET Developer"
                },
                "start_date": "2021-08-04",
                "id": "1313525776161186"
            }
        ]
    }
}
```
</details>

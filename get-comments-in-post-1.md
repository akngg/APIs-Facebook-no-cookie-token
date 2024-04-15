# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get danh sách comment của bài viết (GraphAPI)</summary>


```http
GET http://graph.scanfb.top/graph/{POST_ID}/comments?limit=100&fields=message,from,created_time,attachments,comments&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `{POST_ID}` | `string` | **Bắt buộc**. ID bài viết, dạng hai số có dấu '_' ở giữa |
| `fields` | `string` | Các trường thông tin muốn get |
| `after` | `string` | Paginate |
| `...` | `...` | Cần thêm trường thông tin gì cứ liên hệ Kiệt |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
    "success": true,
    "message": "",
    "data": {
        "data": [
            {
                "message": ",",
                "created_time": "2024-04-13T22:58:59+07:00",
                "id": "7527888420566665"
            },
            {
                "message": ",",
                "created_time": "2024-04-13T23:06:14+07:00",
                "id": "7527912303897610"
            },
            {
                "message": "Hi",
                "created_time": "2024-04-13T23:13:00+07:00",
                "id": "7527935150561992"
            },
            {
                "message": "Buget bao nhiêu",
                "created_time": "2024-04-15T15:21:25+07:00",
                "id": "7534705636551610"
            }
        ],
        "paging": {
            "cursors": {
                "before": "MQZDZD",
                "after": "NAZDZD"
            }
        }
    }
}
```
</details>

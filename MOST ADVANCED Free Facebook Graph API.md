# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>API miễn phí thay thế cho Graph Facebook API</summary>

### URL ban đầu của Graph Facebook API

```http
GET http://graph.facebook.com/{YOUR PATH AND PARAM}...
```

### URL thay thế

```http
GET http://graph.scanfb.top/graph/{YOUR PATH AND PARAM}...&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |

### Hoạt động cho tất cả endpoint của Graph Facebook API

### Response

```json
{
    "success": true,
    "message": "",
    "data": {Graph Facebook API responses}
}
```
</details>

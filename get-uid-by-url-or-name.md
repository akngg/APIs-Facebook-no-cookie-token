# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get UID của link, username, ...</summary>


```http
GET http://graph.scanfb.top/graphql?action=get_uid&input=anhkiet9052&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `action` | `string` | **Cố định**. Chọn API  |
| `input` | `string` | **Bắt buộc**. Link hoặc username của fanpage, nhóm, trang cá nhân |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
    "success": true,
    "message": "",
    "data": 100025113282190
}
```
</details>

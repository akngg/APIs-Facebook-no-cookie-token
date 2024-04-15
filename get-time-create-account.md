# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Ngày tạo tài khoản facebook</summary>


```http
GET http://graph.scanfb.top/graphql?action=check_create_account_date&uid=100025113282190&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `action` | `string` | **Cố định**. Chọn API  |
| `uid` | `string` | **Bắt buộc**. UID tài khoản muốn check |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
  "success": true,
  "message": "",
  "data": "2018-04-20T20:05:07+07:00"
}
```
</details>

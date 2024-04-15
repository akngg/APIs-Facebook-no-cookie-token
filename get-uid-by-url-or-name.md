# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get reactions (cảm xúc) của bài viết</summary>


```http
GET http://graph.scanfb.top/graphql?action=post_reactions&post_id=7523377607684413&cursor=&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `action` | `string` | **Cố định**. Chọn API lấy reactions |
| `post_id` | `string` | **Bắt buộc**. ID bài viết, dạng số, không có dấu '_' |
| `cursor` | `string` |  Request đầu tiên có thể để trống, lấy trong response truyền vào cho request tiếp theo |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

<details>
```json

```
</details>
</details>

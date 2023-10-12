## Chia sẽ bài viết vào nhóm

```http
POST https://graph.facebook.com/groupID/feed
```
<br/>

>Exam: https://graph.facebook.com/123456789/feed

<br/>

| Tham số Body | Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token cá nhân |
| `link` | `string` | `Có` | URL bài viết |
| `message` | `string` | `Không` | Nội dung bài viết |


### Response
```json
{
    "id": "858568104559194_1838286676587327"
}
```

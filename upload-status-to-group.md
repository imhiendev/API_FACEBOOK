## Đăng bài vào nhóm không kèm ảnh

```http
POST https://graph.facebook.com/groupID/feed
```
<br/>

>Exam: https://graph.facebook.com/123456789/feed

<br/>

| Tham số Body | Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token cá nhân |
| `message` | `string` | `Có` | Nội dung bài viết |


### Response
```json
{
    "id": "339909364035155"
}
```

## Đăng bài vào nhóm kèm ảnh

```http
POST https://graph.facebook.com/groupID/photos
```
<br/>

>Exam: https://graph.facebook.com/123456789/photos

<br/>

| Tham số Body| Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token cá nhân |
| `message` | `string` | `Không` | Nội dung bài viết |
| `image` | `string` | `Có` | Đường dẫn ảnh |


### Response
```json
{
    "id": "339909364035155",
    "post_id": "858568104559212_1836502133432128"
}
```

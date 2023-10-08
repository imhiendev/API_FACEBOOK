
## ĐĂNG ẢNH LÊN TRANG CÁ NHÂN

```http
POST https://graph.facebook.com/v13.0/me/photos
```
| Body Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token cá nhân |
| `message` | `string` | Nội dung đăng ảnh |
| `file` | `string` | Đường dẫn ảnh |


### Response
```json
{
    "id": "3398094590451171",
    "post_id": "100007519893105_3398094590451171"
}
```
<br/>

## ĐĂNG ẢNH LÊN PAGE

```http
POST https://graph.facebook.com/v13.0/me/photos
```
| Body Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token page |
| `message` | `string` | Nội dung đăng ảnh |
| `file` | `string` | Đường dẫn ảnh |


### Response
```json
{
    "id": "122097893528073346",
    "post_id": "61552200386006_122097893528073346"
}
```



# API

Những API mẫu sẽ được liệt kê dưới đây

<details>

<summary>API LIKE POST</summary>

## Like bài viết

```http
POST https://graph.facebook.com/idUser_idPost/likes
```
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token của bạn |
| `idUser` | `string` | ID người đăng bài |
| `idPost` | `string` | ID bài viết |


### Response
```text
true
```
</details>


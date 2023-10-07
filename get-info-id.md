
# API

Những API mẫu sẽ được liệt kê dưới đây

<details>

<summary>API GET INFO UID</summary>

## Lấy thông tin id

```http
GET https://graph.facebook.com/userID
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token của bạn |
| `userID` | `string` | ID cần lấy thông tin |

### Respone

```json
{
  "id": "100000691174655",
  "first_name": "Pat",
  "gender": "female",
  "is_employee": false,
  "last_name": "Scheckner",
  "link": "https://www.facebook.com/pat.scheckner",
  "locale": "en_US",
  "name": "Pat Scheckner",
  "timezone": 3,
  "updated_time": "2012-07-31T21:35:07+0000",
  "username": "pat.scheckner"
}
```
</details>

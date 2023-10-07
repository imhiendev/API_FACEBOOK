
# API

Những API mẫu sẽ được liệt kê dưới đây

<details>

<summary>API GET COMMENT</summary>

## Lấy bình luận bài viết

```http
GET https://graph.facebook.com/potstID/comments
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token của bạn |
| `postID` | `string` | **Bắt buộc**. ID bài viết |
| `limit` | `int` | Số bình luận cần lấy trong một lần request |


### Respone
```json
{
    "data": [
        {
            "created_time": "2023-10-07T09:10:56+0000",
            "from": {
                "name": "Nguyễn Nam",
                "id": "100011560725691"
            },
            "message": "Soft này xài khá OK, thường xuyên khuyến mãi, anh em reg cái acc, canh share code cứ redeem vô là được cộng dồn.",
            "can_remove": false,
            "like_count": 0,
            "user_likes": false,
            "id": "2223931101272331"
        },
        {
            "created_time": "2023-10-07T08:40:40+0000",
            "from": {
                "name": "Đạo Vũ",
                "id": "100011349600991"
            },
            "message": "Cám ơn bác nhé, tí về thử sau 🫰",
            "can_remove": false,
            "like_count": 1,
            "user_likes": false,
            "id": "2223918717940236"
        },
        {
            "created_time": "2023-10-07T08:50:58+0000",
            "from": {
                "name": "Kha Duy",
                "id": "100048150274725"
            },
            "message": "macos dùng được kh bác",
            "can_remove": false,
            "like_count": 0,
            "user_likes": false,
            "id": "2223922764606498"
        }
  ]
}
```
</details>


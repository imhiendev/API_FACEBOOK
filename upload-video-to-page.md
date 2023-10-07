
# API

Những API mẫu sẽ được liệt kê dưới đây

<details>

<summary>API GET VIDEO</summary>

## Lấy video từ page

```http
GET https://graph.facebook.com/v13.0/page_id/feed?fields=source,message
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token của bạn |
| `page_id` | `string` | Thay thế thành id cần lấy dữ liệu |

### Respone

```json
{
   "data": [
      {
         "source": "https://scontent.fsgn5-11.fna.fbcdn.net/v/t42.1790-2/10000000_350124847385985_6026143748923098927_n.mp4?_nc_cat=111&ccb=1-7&_nc_sid=985c63&efg=eyJybHIiOjU4MSwicmxhIjo0MDk2LCJ2ZW5jb2RlX3RhZyI6InN2ZV9zZCJ9&_nc_ohc=1jvg9D-2Ee4AX_Q1KIG&rl=581&vabr=323&_nc_ht=scontent.fsgn5-11.fna&oh=00_AfCnFWvvayD92z9OejH-HnOrAyraj_hLin26m85bTgonoA&oe=652664AC",
         "message": "Review Phim  H\u1ee3p \u0110\u1ed3ng H\u00f4n Nh\u00e2n T\u1eadp Cu\u1ed1i \n#H\u1ee3p\u0110\u1ed3ngH\u00f4nNh\u00e2n  #reviewphim",
         "id": "108618388959890_173023105844632"
      },
      {
         "source": "https://scontent.fsgn5-12.fna.fbcdn.net/v/t42.1790-2/10000000_968107100949960_160179432361630306_n.mp4?_nc_cat=103&ccb=1-7&_nc_sid=985c63&efg=eyJybHIiOjQzOSwicmxhIjoxODY2LCJ2ZW5jb2RlX3RhZyI6InN2ZV9zZCJ9&_nc_ohc=IfSGPRn60oYAX-yChB3&rl=439&vabr=244&_nc_ht=scontent.fsgn5-12.fna&oh=00_AfDiPq3tdGaj6fHFnR2S2_iez6jgwl2FPvXzD_xBGAmYMA&oe=65269B2F",
         "message": "Review Phim  H\u1ee3p \u0110\u1ed3ng H\u00f4n Nh\u00e2n T\u1eadp 8\n#H\u1ee3p\u0110\u1ed3ngH\u00f4nNh\u00e2n  #reviewphim",
         "id": "108618388959890_173018082511801"
      }
}      
```
</details>

<details>

<summary>API UPLOAD VIDEO</summary>

## Đăng video

```http
POST https://graph-video.facebook.com/v18.0/me/videos
```

| Body Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token của bạn |
| `file_url` | `string` | Thay thế thành giá trị source video |
| `description` | `string` | Thay thế thành giá trị message |

### Respone
```json
{
    "error": {
        "message": "An unknown error has occurred.",
        "type": "OAuthException",
        "code": 1,
        "fbtrace_id": "AUbytnp1v-crfgnXYk3V3eX"
    }
}
```
</details>

**_LƯU Ý: TUY LÀ THÔNG BÁO LỖI NHƯNG VIDEO VẪN ĐƯỢC XỬ LÝ VÀ ĐĂNG LÊN PAGE THEO TOKEN_**

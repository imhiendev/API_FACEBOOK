# Setup
+ Token page. Nếu không biết lấy token page, bấm [vào đây](https://github.com/imhiendev/get-token-page-facebook) để biết cách.


## Lấy list tin nhắn trên page

```http
GET https://graph.facebook.com/v12.0/me?fields=conversations
```

| Tham số | Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token page |

<br/>

>Ví dụ: https://graph.facebook.com/v12.0/me?fields=conversations&access_token=EAABWnanfkakxxxxxxx

### Response

```json
{
  "conversations": {
    "data": [
      {
        "id": "t_6861775753867082",
        "link": "/136823816993251/inbox/1228007537874868/",
        "updated_time": "2023-09-20T09:07:45+0000"
      },
      {
        "id": "t_3523788767936812",
        "link": "/136823816993251/inbox/1227941881214767/",
        "updated_time": "2023-09-20T05:31:33+0000"
      },
      {
        "id": "t_2585447901617684",
        "link": "/136823816993251/inbox/1220992375243051/",
        "updated_time": "2023-09-05T12:47:52+0000"
      }
  ]
}
```
## Lấy thông tin tin nhắn

```http
GET https://graph.facebook.com/v12.0/conversionID?fields=messages{from}
```



| Tham số | Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token page |


<br/>

>Ví dụ: https://graph.facebook.com/v12.0/t_6861775753867082?fields=messages{from}&access_token=EAABWnanfkakxxxxxxx

### Response

```json
{
  "messages": {
    "data": [
      {
        "from": {
          "name": "STAR SAT",
          "email": "136823816993251@facebook.com",
          "id": "136823816993251"
        },
        "id": "m_W8U87eYB-6LOlTKYHPmxC4RvXBNxK6-SQDKWFVYL53KKr0jJYiHGaOq2BtwdfTzYnutnufAcvKCwvdjOmu6Qfa"
      },
      {
        "from": {
          "name": "مصطفی مجددی",
          "email": "6215289098575526@facebook.com",
          "id": "6215289098575526"
        },
        "id": "m_REK7h79lsRp_4hsDx4qLmIRvXBNxK6-SQDKWFVYL53Lhw8Gn1nP1X8cZd9EcOBm243hmh3rHcvQHKtzrDSBsaw"
      }
    ]
}
```
## Lấy thông tin UID

```http
GET https://graph.facebook.com/userID
```

| Tham số | Loại     |Bắt buộc     | Mô tả                |
| :-------- | :------- | :---- | :------------------------- |
| `access_token` | `string` | `Có` | Token page |

<br/>

>Ví dụ: https://graph.facebook.com/6215289098575526

### Response

```json
{
  "id": "6215289098575526",
  "about": "﮼پناه‌میبرم‌به‌خدایی‌که‌قرارِ‌دل‌ماست..♥️",
  "birthday": "10/19/1994",
  "education": [
    {
      "school": {
        "id": "268326953203170",
        "name": "Kardan University"
      },
      "type": "College",
      "id": "2265877377061297"
    },
    {
      "school": {
        "id": "115143731830081",
        "name": "Naderia High School"
      },
      "type": "High School",
      "id": "1529063987409310"
    }
  ],
  "first_name": "مصطفی",
  "gender": "male",
  "hometown": {
    "id": "113507521993978",
    "name": "Panjshir, Parvan, Afghanistan"
  },
  "is_employee": false,
  "languages": [
    {
      "id": "110159765673211",
      "name": "فارسی"
    }
  ],
  "last_name": "مجددی",
  "location": {
    "id": "102164239825190",
    "name": "کابل، افغانستان"
  },
  "locale": "en_US",
  "mobile_phone": "+93794505090",
  "name": "مصطفی مجددی",
  "relationship_status": "In a relationship",
  "timezone": 4.5,
  "updated_time": "2023-10-09T21:30:47+0000",
  "username": "mustafamujaddadi",
  "work": [
    {
      "end_date": "0000-00",
      "employer": {
        "id": "435350637198128",
        "name": "F . V . P"
      },
      "start_date": "2014-05-22",
      "id": "2265878897061145"
    }
  ]
}
```

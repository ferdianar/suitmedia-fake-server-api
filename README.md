# Suitmedia Fake Server API

Untuk mempermudah test fake data ketika di production. Ini saya punya inisiatif untuk membuat fake server dari **comments json** menggunakan Heroku App. 
Sehingga peoject yang sudah saya deploy ke vercel, nanti mengambil data nya ke url Fake Server URL ( https://suitmedia-fake-server-api.herokuapp.com/comments ).

Untuk data comments.json nya seperti ini

```json
{
    "comments": [{
            "id": "fa1ca3c1-cc1e-4ed9-86b8-f60d8312d499",
            "author": "Neal Topham",
            "avatar": "http://lorempixel.com/100/100/people/1/",
            "images": "https://placeimg.com/640/480/people/sepia",
            "date": "2017-02-08T00:30:05.552Z",
            "message": "Mungkin ada fenomena paranormal yang tidak bisa dijelaskan. Lebih baik nyala mati sendiri daripada tidak nyala sama sekali",
            "point": 3,
            "replies": [{
                "id": "4ba9a8d1-cbe9-4906-ac23-0030f5df027e",
                "author": "Dyan Shankin",
                "avatar": "http://lorempixel.com/100/100/people/2/",
                "date": "2017-02-08T00:33:20.369Z",
                "message": "Confirm, itu kemungkinan aktivitas paranormal.",
                "point": 0
            }]
        },
        {
            "id": "9b3d6fe2-e3fc-47c6-b09a-f2b40547b101",
            "author": "Jacquelyne Garrity",
            "avatar": "http://lorempixel.com/100/100/people/2/",
            "images": "https://placeimg.com/640/480/people/sepia",
            "date": "2017-02-08T00:32:18.214Z",
            "message": "Saya mengalami hal serupa. Laptop yang digunakan Toshiba L645. Tolong infonya.",
            "point": 0,
            "replies": [{
                    "id": "e157bcd4-68d7-4d2a-ade1-da50f0913daf",
                    "author": "Shella Tamashiro",
                    "avatar": "http://lorempixel.com/100/100/people/1/",
                    "date": "2017-02-09T00:33:20.369Z",
                    "message": "Ada kemungkinan ini masalah virus. Coba dilakukan virus scan menggunakan software anti virus.",
                    "point": 1
                },
                {
                    "id": "ff441e8a-7465-4527-bd9a-ed6d3ad5fdef",
                    "author": "Marcelino Stangle",
                    "avatar": "http://lorempixel.com/100/100/people/1/",
                    "date": "2017-02-09T00:37:38.411Z",
                    "message": "Setuju",
                    "point": 1
                }
            ]
        },
        {
            "id": "27526171-1236-4785-a67f-72b48989e3ff",
            "author": "Lawanda Schey",
            "avatar": "http://lorempixel.com/100/100/people/3/",
            "images": "https://placeimg.com/640/480/people/sepia",
            "date": "2017-02-09T00:32:18.214Z",
            "message": "Apakah ada solusi lain? Sudah dicoba untuk scan virus tapi kasus ini tetap ada.",
            "point": 1,
            "replies": []
        }
    ]
}
```

Dengan memfetching data dari api tersebut, hasil data nya seperti di atas yang nantinya siap untuk di render ke React HTML Elements

Terima Kasih .....
**Ferdian Ahmad R**

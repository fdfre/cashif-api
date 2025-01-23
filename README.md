# API Documentation

## Get all manufacturers

- **Endpoint:** `https://cashif.online/back-end/public/api/all-manufacturers`
- **Method:** `GET`


#### Response
- **Status Code:** 200 OK
- **Body:**
```json
[
    {
        "id": 1,
        "title": "1984",
        "author": "George Orwell",
        "published_date": "1949-06-08"
    },
    {
        "id": 2,
        "title": "To Kill a Mockingbird",
        "author": "Harper Lee",
        "published_date": "1960-07-11"
    }
]


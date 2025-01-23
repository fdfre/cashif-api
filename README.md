# API Documentation

## Get all manufacturers

- **Endpoint:** `https://cashif.online/back-end/public/api/all-manufacturers`
- **Method:** `GET`


#### Response

```json
{
    "manufacturers": [
        {
            "id": 1,
            "manufacture_name": "Toyota"
        },
        {
            "id": 2,
            "manufacture_name": "Kia"
        },
        {
            "id": 3,
            "manufacture_name": "Audi"
        },
    ]
}
```

## Get models by manufacture id

- **Endpoint:** `https://cashif.online/back-end/public/api/all-models-by-manufacture-id/{manufactureId}`
- **Method:** `GET`
- **Parameter:** `manufactureId`

#### Response

```json
{
    "manufacturers": [
        {
            "id": 1,
            "manufacture_name": "Toyota"
        },
        {
            "id": 2,
            "manufacture_name": "Kia"
        },
        {
            "id": 3,
            "manufacture_name": "Audi"
        },
    ]
}
```


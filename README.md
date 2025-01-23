# API Documentation

## Get all manufacturers (ماركة السيارة)

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

<br><br>

## Get models by manufacture id (فئة السيارة)

- **Endpoint:** `https://cashif.online/back-end/public/api/all-models-by-manufacture-id/{manufactureId}`
- **Method:** `GET`
- **Parameter:** `manufactureId`

#### Response

```json
{
    "carModels": [
        {
            "id": 3,
            "model_name": "اكورد - Accord"
        },
        {
            "id": 5,
            "model_name": "انتيجرا - Integra"
        },
        {
            "id": 1,
            "model_name": "اوديسي - Odyssey"
        },
    ]
}
```

<br><br>

## Year (السنة)

```javascript
  if (yearValue >= 2015) {
    year_id = 2;
  } else {
    year_id = 1;
  }
```

<br><br>

## Get plans & prices by model id and year id

- **Endpoint:** `https://cashif.online/back-end/public/api/all-plans-prices-by-model-id/{modelId}/and-year-id/{yearId}`
- **Method:** `GET`
- **Parameter:** `modelId` and `yearId`

#### Response

```json
[
    {
        "manufacturer": "Toyota",
        "model": "كامري - Camry",
        "car_model_id": "56",
        "year_id": "2",
        "prices": [
            {
                "price_id": 0,
                "plan": "شامل",
                "price": "560.00"
            },
            {
                "price_id": 1,
                "plan": "أساسي",
                "price": "430.00"
            },
            {
                "price_id": 2,
                "plan": "محركات",
                "price": "300.00"
            }
        ]
    }
]
```



<br><br>

## Note about "نوع طلب الفحص"

### In cashif we have 2 type:

- **1:** `فحص ما قبل الشراء`
- **2:** `فحص مخدوم`

<br><br>

## Note about plans links:

If user select `فحص ما قبل الشراء` the links of plans should be:

`https://cashif.cc/pay/?plan={plan}&year_id={year_id}&car_model_id={car_model_id}&price_id={price_id}&affiliate=mshrai` 

- **Parameter:** `plan` `year_id` `car_model_id` `price_id`

<br>

If user select `فحص مخدوم` only 2 plans should show `شامل` , `أساسي` and the links of plans should be:

`https://cashif.cc/check-it/receipt/?plan={plan}&year_id={year_id}&car_model_id={car_model_id}&price_id={price_id}&affiliate=mshrai` 

- **Parameter:** `plan` `year_id` `car_model_id` `price_id`













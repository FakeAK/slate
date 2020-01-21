# Stores

<!-- GET /stores/all
GET /stores/:store_id-->

## Get All Stores by Query

```json
{
    "message": null,
    "payload": {
        "friends": [
            {
                "id": 171,
                "title": "LA VAUJANY",
                "city": "Vaujany, Isère",
                "photo_cover": "https://bikenconnect.com/uploads/events/photo_cover/171/850_et0n93ae4682e5y1vs7131219042633.jpg",
                "from": "2020-07-01",
                "from_time": "0:00",
                "isRegisterEnabled": 0,
                "disciplines": [
                    "Road"
                ],
                "lien_inscription": null,
                "interestedPeopleCount": 0,
                "registerBySNC": false
            },
            ...
        ]
    }
```

Get all friends from current authenticated user. This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/stores/all`

<aside class="success">
Return a 200 status code with a list of teams.
</aside>

## Get Store by Id

```json
{
    "message": null,
    "payload": {
        "friends": [
            {
                "id": 171,
                "title": "LA VAUJANY",
                "city": "Vaujany, Isère",
                "photo_cover": "https://bikenconnect.com/uploads/events/photo_cover/171/850_et0n93ae4682e5y1vs7131219042633.jpg",
                "from": "2020-07-01",
                "from_time": "0:00",
                "isRegisterEnabled": 0,
                "disciplines": [
                    "Road"
                ],
                "lien_inscription": null,
                "interestedPeopleCount": 0,
                "registerBySNC": false
            },
            ...
        ]
    }
```

Get all friends from current authenticated user. This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/stores/:store_id`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
store_id | Integer | Required. The id of the store to search.

<aside class="success">
Return a 200 status code with a list of teams.
</aside>
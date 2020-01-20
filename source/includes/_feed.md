# Feed

## Get Events

```json
{
    "message": null,
    "payload": {
        "events": [
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

Get the events on the home page.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/activity/events`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
page | Integer | If this parameter is omitted, default value is 1.
firstLoad | Boolean | If this parameter is omitted, default value is true.

<aside class="success">
Return a 200 status code with a list of events.
</aside>

## Get Trainings

```json
{
    "message": null,
    "payload": [
        {
            "id": 3789,
            "title": "Sortie matinale si la météo est bonne",
            "city": "Rue des Moques Tonneaux, 91540 Ormoy, France",
            "photo_cover": "https://bikenconnect.com/uploads/trainings/photo/3789/450_9e70efd7473e85b873ed3a3ac6b580b5.jpg",
            "from": "2020-01-21T06:00:00.000Z",
            "disciplines": [
                "Road"
            ],
            "lat": "48.57265770",
            "lng": "2.45445540",
            "nbParticipant": 1
        },
        ...
    ]
}
```

Get the trainings on the home page.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/activity/trainings`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
page | Integer | If this parameter is omitted, default value is 1.
longitude | Float | The user's longitude, in order to get him the closest trainings.
latitude | Float | The user's latitude, in order to get him the closest trainings.

<aside class="success">
Return a 200 status code with a list of trainings.
</aside>

## Get Stores

```json
{
    "message": null,
    "payload": [
        {
            "id": 9,
            "logo": "eU31ysW67eXtV4Z0va5n28Ye9130120012411.jpg",
            "name": "Cycles Laurent",
            "city": "9 Boulevard Voltaire,75011 Paris",
            "description": "Large choix de vélos de tout type, accessoires et équipements, ventes d'occasion dans un magasin spécialisé.",
            "lat": 48.86616898,
            "lng": 2.3664,
            "distanceFromUser": 5.59040083877893,
            "photo_cover": "https://bikenconnect.com/uploads/eU31ysW67eXtV4Z0va5n28Ye9130120012411.jpg",
            "type": "Store"
        },
        ...
    ]
}
```

Get the closest stores for the home page.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/activity/stores`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
page | Integer | If this parameter is omitted, default value is 1.
longitude | Float | The user's longitude, in order to get him the closest stores.
latitude | Float | The user's latitude, in order to get him the closest stores.

<aside class="success">
Return a 200 status code with a list of stores.
</aside>

## Get Friends Recommandations

```json
{
    "message": null,
    "payload": [
        {
            "id": 6115,
            "fullname": "Pierre Micheau",
            "photo": "https://bikenconnect.com/uploads/users/avatar/6115/100_square_ea2d1733513df69366b4203b760b5f74.jpg"
        },
        {
            "id": 188,
            "fullname": "Philippe RIVIERE",
            "photo": "https://bikenconnect.com/uploads/users/avatar/188/100_square_5839f4d460435b9374425dab8ae90566_tmp.jpg"
        },
        ...
    ]
}
```

Get the friends recommandations for the home page.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/activity/friendsSuggestion`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
page | Integer | If this parameter is omitted, default value is 1.

<aside class="success">
Return a 200 status code with a list of friends recommandations.
</aside>

## Get Teams Recommandations

```json
{
    "message": null,
    "payload": [
        {
            "id": 370,
            "photo": "https://bikenconnect.com/uploads/teams/photo/370/450_image-092d374f-eee0-4387-97ff-0895623efce2.jpg",
            "name": "PUC",
            "lat": "48.81955050",
            "lng": "2.34582290",
            "distanceFromUser": 1.3270265158448808
        },
        {
            "id": 157,
            "photo": "https://bikenconnect.com/uploads/teams/photo/157/450_CCD35E1E-6A02-4DAC-B73A-4FEA78F5BFDB.jpg",
            "name": "Paris Cycling Group",
            "lat": "48.82424910",
            "lng": "2.31874110",
            "distanceFromUser": 3.376410527939169
        },
        ...
    ]
}
```

Get the teams recommandations for the home page.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/activity/teamsSuggestion`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
page | Integer | If this parameter is omitted, default value is 1.
longitude | Float | The user's longitude, in order to get him the closest teams.
latitude | Float | The user's latitude, in order to get him the closest teams.

<aside class="success">
Return a 200 status code with a list of teams recommandations.
</aside>
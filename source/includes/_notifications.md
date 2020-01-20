# Notifications

<aside class="notice">
All the endpoints need an access token.
</aside>

## Get Notifications List

```json
{
    "message": null,
    "payload": [
        {
            "id": 76806,
            "user_id": 187,
            "sender_id": 623,
            "created": "2020-01-17T08:46:13.000Z",
            "text": "",
            "action": "vous invite à l'entraînement",
            "url": "/trainings/view/5324",
            "read": 1,
            "params": "Sortie RUGISSANTS du Jeudi",
            "plugin": "",
            "sender": {
                "avatar": "https://bikenconnect.com/uploads/users/avatar/623/100_square_ca8d0deb33c797e58e1b13ec768f285e.jpg",
                "fullName": "Georges  Extrat "
            },
            "itemID": "5324",
            "item": {
                "id": 5324,
                "title": "Sortie RUGISSANTS du Jeudi",
                "image": "https://bikenconnect.com/uploads/trainings/photo/5324/450_787083785dc434a64f90a8a656257e39.png",
                "type": "training"
            }
        },
        ...
    ]
}
```

### HTTP Request

`GET https://api.sportsnconnect.com/notifications/`

## Mark all notification as read

### HTTP Request
`PUT https://api.sportsnconnect.com/notifications/`


## Search a notification

### HTTP Request
`GET https://api.sportsnconnect.com/notifications/search`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
q | String | A name to search.

## Get notifications unread (count)

```json
{
    "message": null,
    "payload": {
        "count": 26
    },
    "status": 200
}
```

### HTTP Request

`GET https://api.sportsnconnect.com/notifications/count`

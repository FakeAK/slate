# Friends

<!-- 
POST /friends/requests/:friendId -->

## Get All Friends

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

`GET https://api.sportsnconnect.com/friends`

<aside class="success">
Return a 200 status code with a list of teams.
</aside>

## Add New Friend

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

Add a friend for current authenticated user. This requests needs a JWT token to work.

### HTTP Request

`POST https://api.sportsnconnect.com/friends`

<aside class="success">
Return a 200 status code with a list of teams.
</aside>

## Get All Friend Requests

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

Get all friend requests for current authenticated user. This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/friends/requests`

<aside class="success">
Return a 200 status code with a list of teams.
</aside>

## Send a Friend Request

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

Send a friend request to a user by its id from current authenticated user. This requests needs a JWT token to work.

### HTTP Request

`POST https://api.sportsnconnect.com/friends/requests/:friendId`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
friendId | Integer | Required. The id of the user to send a friend request to.

<aside class="success">
Return a 200 status code with a list of teams.
</aside>
# Teams

## Create team

> Success:
```json
{
  "message": null,
  "status": 200,
  "payload": {
    "id":  0,
    "category_id":  0,
    "name": "Team",
    "user_id": 1,
    "description": "Description",
    "distance": 10,
    "level_id": 0,
    "disciplines": "[1, 2, 3]",
    "type": 0,
    "photo": "http://....",
    "address": "Adresse",
    "city": "Ville",
    "country": "Pays",
    "photo_cover": "http://....",
    "team_user_count": 1,
    "kilometer_count": 0,
    "training_count": 0,
    "status": 0,
    "lat": 0.00,
    "lng": 0.00,
    "approved": 1,
    "created": "2020-06-01",
    "photo_count": 0,
    "topic_count": 0,
    "video_count": 0,
    "event_count": 0,
    "featured": 0,
    "group_types": 0,
    "website": "http://....",
    "facebook": "http://.....",
    "twitter": "http://....",
    "instagram": "http://....",
    "strava": "http://.....",
    "linkedin": "http://....",
    "bike1_id": 0,
    "privacy_type": 0,
    "conversation_id": 10
  }
}
```

> Error :
```json
{
  "message": "An error occured",
  "status": 400,
  "errors": {}
}
```
This endpoint create a team.

### HTTP Request

`POST https://api.sportsnconnect.com/team`

### Query Parameters
Parameter | Description
--------- | -----------
name | Team's name
address | Local address
level | Team level
disciplines | Array of disciplines practices by the team
photo | Team photo
photo_cover | Team photo_cover
city | City of the team
country | Country of the team
lat | Latitude of the address
lng | Longitude of the address
user_id | Id of the owner

<aside class="success">
If the call succeeds you'll get the team data.
</aside>

## Get all teams depending of a name
> Success:
```json
{
  "message": null,
   "status": 200,
   "payload": [
   {
       "id":  0,
           "category_id":  0,
           "name": "Team",
           "user_id": 1,
           "description": "Description",
           "distance": 10,
           "level_id": 0,
           "disciplines": "[1, 2, 3]",
           "type": 0,
           "photo": "http://....",
           "address": "Adresse",
           "city": "Ville",
           "country": "Pays",
           "photo_cover": "http://....",
           "team_user_count": 1,
           "kilometer_count": 0,
           "training_count": 0,
           "status": 0,
           "lat": 0.00,
           "lng": 0.00,
           "approved": 1,
           "created": "2020-06-01",
           "photo_count": 0,
           "topic_count": 0,
           "video_count": 0,
           "event_count": 0,
           "featured": 0,
           "group_types": 0,
           "website": "http://....",
           "facebook": "http://.....",
           "twitter": "http://....",
           "instagram": "http://....",
           "strava": "http://.....",
           "linkedin": "http://....",
           "bike1_id": 0,
           "privacy_type": 0,
           "conversation_id": 10
},
{
"id":  0,
    "category_id":  0,
    "name": "Team",
    "user_id": 1,
    "description": "Description",
    "distance": 10,
    "level_id": 0,
    "disciplines": "[1, 2, 3]",
    "type": 0,
    "photo": "http://....",
    "address": "Adresse",
    "city": "Ville",
    "country": "Pays",
    "photo_cover": "http://....",
    "team_user_count": 1,
    "kilometer_count": 0,
    "training_count": 0,
    "status": 0,
    "lat": 0.00,
    "lng": 0.00,
    "approved": 1,
    "created": "2020-06-01",
    "photo_count": 0,
    "topic_count": 0,
    "video_count": 0,
    "event_count": 0,
    "featured": 0,
    "group_types": 0,
    "website": "http://....",
    "facebook": "http://.....",
    "twitter": "http://....",
    "instagram": "http://....",
    "strava": "http://.....",
    "linkedin": "http://....",
    "bike1_id": 0,
    "privacy_type": 0,
    "conversation_id": 10
}
  ]
}
```
> Error :
```json
{
  "message": "error message",
  "status": 400,
  "payload": null
}
```

Get all teams who can match a name

### HTTP Request

`GET https://api.sportsnconnect.com/team/all?name=`

### Query Parameters
Parameter | Description
--------- | -----------
name | Team name

<aside class="success">
Returns an array with all team who match the name
</aside>

## Get all teams
> Success:
```json
{
  "message": null,
   "status": 200,
   "payload": [
   {
       "id":  0,
           "category_id":  0,
           "name": "Team",
           "user_id": 1,
           "description": "Description",
           "distance": 10,
           "level_id": 0,
           "disciplines": "[1, 2, 3]",
           "type": 0,
           "photo": "http://....",
           "address": "Adresse",
           "city": "Ville",
           "country": "Pays",
           "photo_cover": "http://....",
           "team_user_count": 1,
           "kilometer_count": 0,
           "training_count": 0,
           "status": 0,
           "lat": 0.00,
           "lng": 0.00,
           "approved": 1,
           "created": "2020-06-01",
           "photo_count": 0,
           "topic_count": 0,
           "video_count": 0,
           "event_count": 0,
           "featured": 0,
           "group_types": 0,
           "website": "http://....",
           "facebook": "http://.....",
           "twitter": "http://....",
           "instagram": "http://....",
           "strava": "http://.....",
           "linkedin": "http://....",
           "bike1_id": 0,
           "privacy_type": 0,
           "conversation_id": 10
},
{
"id":  0,
    "category_id":  0,
    "name": "Team",
    "user_id": 1,
    "description": "Description",
    "distance": 10,
    "level_id": 0,
    "disciplines": "[1, 2, 3]",
    "type": 0,
    "photo": "http://....",
    "address": "Adresse",
    "city": "Ville",
    "country": "Pays",
    "photo_cover": "http://....",
    "team_user_count": 1,
    "kilometer_count": 0,
    "training_count": 0,
    "status": 0,
    "lat": 0.00,
    "lng": 0.00,
    "approved": 1,
    "created": "2020-06-01",
    "photo_count": 0,
    "topic_count": 0,
    "video_count": 0,
    "event_count": 0,
    "featured": 0,
    "group_types": 0,
    "website": "http://....",
    "facebook": "http://.....",
    "twitter": "http://....",
    "instagram": "http://....",
    "strava": "http://.....",
    "linkedin": "http://....",
    "bike1_id": 0,
    "privacy_type": 0,
    "conversation_id": 10
}
  ]
}
```
> Error :
```json
{
  "message": "error message",
  "status": 400,
  "payload": null
}
```

Get all teams who can match a name

### HTTP Request

`GET https://api.sportsnconnect.com/team/all`

<aside class="success">
Returns an array with all team
</aside>

## Get all teams
> Success:
```json
{
  "message": null,
   "status": 200,
   "payload": {
    "id":  0,
    "category_id":  0,
    "name": "Team",
    "user_id": 1,
    "description": "Description",
    "distance": 10,
    "level_id": 0,
    "disciplines": "[1, 2, 3]",
    "type": 0,
    "photo": "http://....",
    "address": "Adresse",
    "city": "Ville",
    "country": "Pays",
    "photo_cover": "http://....",
    "team_user_count": 1,
    "kilometer_count": 0,
    "training_count": 0,
    "status": 0,
    "lat": 0.00,
    "lng": 0.00,
    "approved": 1,
    "created": "2020-06-01",
    "photo_count": 0,
    "topic_count": 0,
    "video_count": 0,
    "event_count": 0,
    "featured": 0,
    "group_types": 0,
    "website": "http://....",
    "facebook": "http://.....",
    "twitter": "http://....",
    "instagram": "http://....",
    "strava": "http://.....",
    "linkedin": "http://....",
    "bike1_id": 0,
    "privacy_type": 0,
    "conversation_id": 10
  }
}
```
> Error :
```json
{
  "message": "Team not found.",
  "status": 404,
  "payload": null
}
```

Get team by ID

### HTTP Request

`GET https://api.sportsnconnect.com/team/:teamId`

### Query Parameters
Parameter | Description
--------- | -----------
teamId | Team id

<aside class="success">
Returns the team
</aside>

## Get team users

This endpoint get all the users of a specific team.

> Success :
```json
{
  "message": null,
  "status": 201,
  "payload": [
    {
    
    },
     {
     
    }
  ]
}
```

> Error :
```json
{
  "message": "Team not found.",
  "status": 404,
  "payload": null
}
```

### HTTP Request

`GET https://api.sportsnconnect.com/team/:teamId/users`

### Query Parameters
Parameter | Description
--------- | -----------
teamId | Team id

<aside class="success">
Returns the users of the team
</aside>

## Get all teams of the user
> Success:
```json
{
  "message": null,
   "status": 200,
   "payload": [
   {
       "id":  0,
           "category_id":  0,
           "name": "Team",
           "user_id": 1,
           "description": "Description",
           "distance": 10,
           "level_id": 0,
           "disciplines": "[1, 2, 3]",
           "type": 0,
           "photo": "http://....",
           "address": "Adresse",
           "city": "Ville",
           "country": "Pays",
           "photo_cover": "http://....",
           "team_user_count": 1,
           "kilometer_count": 0,
           "training_count": 0,
           "status": 0,
           "lat": 0.00,
           "lng": 0.00,
           "approved": 1,
           "created": "2020-06-01",
           "photo_count": 0,
           "topic_count": 0,
           "video_count": 0,
           "event_count": 0,
           "featured": 0,
           "group_types": 0,
           "website": "http://....",
           "facebook": "http://.....",
           "twitter": "http://....",
           "instagram": "http://....",
           "strava": "http://.....",
           "linkedin": "http://....",
           "bike1_id": 0,
           "privacy_type": 0,
           "conversation_id": 10
},
{
"id":  0,
    "category_id":  0,
    "name": "Team",
    "user_id": 1,
    "description": "Description",
    "distance": 10,
    "level_id": 0,
    "disciplines": "[1, 2, 3]",
    "type": 0,
    "photo": "http://....",
    "address": "Adresse",
    "city": "Ville",
    "country": "Pays",
    "photo_cover": "http://....",
    "team_user_count": 1,
    "kilometer_count": 0,
    "training_count": 0,
    "status": 0,
    "lat": 0.00,
    "lng": 0.00,
    "approved": 1,
    "created": "2020-06-01",
    "photo_count": 0,
    "topic_count": 0,
    "video_count": 0,
    "event_count": 0,
    "featured": 0,
    "group_types": 0,
    "website": "http://....",
    "facebook": "http://.....",
    "twitter": "http://....",
    "instagram": "http://....",
    "strava": "http://.....",
    "linkedin": "http://....",
    "bike1_id": 0,
    "privacy_type": 0,
    "conversation_id": 10
}
  ]
}
```
> Error :
```json
{
  "message": "error message",
  "status": 400,
  "payload": null
}
```

Get all teams of the user

### HTTP Request

`GET https://api.sportsnconnect.com/team/users/:user_id`

### Query Parameters
Parameter | Description
--------- | -----------
user_id | User id

<aside class="success">
Returns an array with all team where the user is
</aside>

## Delete a team

> Success :
```json
{
  "payload": null,
  "message": "Team deleted.",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 501
}
```
```json
{
  "payload": null,
  "message": "Access refused.",
  "status": 401
}
```
```json
{
  "payload": null,
  "message": "Team not found.",
  "status": 404
}
```

This endpoint delete a specific team.

### HTTP Request

`DELETE https://api.sportsnconnect.com/team/:team_id/users/:user_id`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

<aside class="success">
The team is deleted
</aside>

## Join a team

> Success :
```json
{
  "payload": null,
  "message": "user joined team.",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 400
}
```

This endpoint allow the user to join a team

### HTTP Request

`PUT https://api.sportsnconnect.com/team/:team_id/users/:user_id/join`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

## Ask to join a team

> Success :
```json
{
  "payload": null,
  "message": "user asked to join the team.",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 400
}
```

This endpoint allow the user to ask for join a team

### HTTP Request

`POST https://api.sportsnconnect.com/team/:team_id/users/:user_id/ask`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

## Add an administrator

> Success :
```json
{
  "payload": null,
  "message": "user is now admin.",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 400
}
```

This endpoint allow to set a user admin

### HTTP Request

`PUT https://api.sportsnconnect.com/team/:team_id/users/:user_id/admin`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

## Remove a admin

> Success :
```json
{
  "payload": null,
  "message": "user leave admin",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 400
}
```

This endpoint allow to remove a admin

### HTTP Request

`PUT https://api.sportsnconnect.com/team/:team_id/users/:user_id/admin/leave`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

## Leave a team

> Success :
```json
{
  "payload": null,
  "message": "user leaved team.",
  "status": 201
}
```
> Errors :
```json
{
  "payload": null,
  "message": "An error occured...",
  "status": 400
}
```

This endpoint allow the user to leave a team

### HTTP Request

`DELETE https://api.sportsnconnect.com/team/:team_id/users/:user_id/leave`

### Query Parameters

Parameter | Description
--------- | -----------
team_id | team id
user_id | user id

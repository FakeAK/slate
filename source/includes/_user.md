# User

<!-- PUT /users/me -->

## Get All Users

```json
{
    "message": null,
    "payload": {
        "users": [
            {
                "id": 14400,
                "name": "Vincent Ducloup",
                "email": "useremail@test.fr",
                "password": "the_user_password",
                "salt": null,
                "role_id": 2,
                "avatar": "avatar_url",
                "photo": "photo_url",
                "created": "2019-12-13T10:33:15.000Z",
                "last_login": "2019-12-13T10:33:15.000Z",
                "photo_count": 2,
                "friend_count": 1,
                "notification_count": 0,
                "friend_request_count": 0,
                "blog_count": 0,
                "topic_count": 0,
                "group_count": 0,
                "event_count": 0,
                "conversation_user_count": 41,
                "video_count": 0,
                "gender": "Male",
                "birthday": "1997-04-15",
                "active": 1,
                "confirmed": 1,
                "code": "",
                "notification_email": 1,
                "timezone": "Europe/Paris",
                "ip_address": "ip_address",
                "privacy": 1,
                "username": "",
                "about": "",
                "featured": 0,
                "lang": "",
                "hide_online": 0,
                "cover": "",
                "approved": 1,
                "is_social": 0,
                "has_active_subscription": 0,
                "receive_message_from_non_friend": 1,
                "send_email_when_send_message": 1,
                "request_friend_email": 1,
                "notification_setting": null,
                "profile_type_id": 1,
                "first_name": "Vincent",
                "last_name": "Ducloup",
                "phone": "0666666666",
                "facebook_link": "",
                "twitter_handle": "",
                "instagram_handle": "",
                "strava_handle": "",
                "linkedin_handle": "",
                "disciplines": "11,1,2,3,4,6",
                "distance": 0,
                "level_id": 1,
                "lat": "0.00000000",
                "lng": "0.00000000",
                "kilometer_count": 0,
                "training_count": 0,
                "team_count": 0,
                "address": "Rue de Rivoli",
                "city": "Paris",
                "state": "",
                "country": "France",
                "bike1_id": 0,
                "is_pro": 0,
                "social_avatar": "",
                "magasin": 0,
                "postal_code": 75001,
                "user_license": null
            },
            ...
        ]
    }
```

Get all users.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/users/all`

<aside class="success">
Return a 200 status code with a list of users.
</aside>

## Get Current User

```json
{
    "message": null,
    "payload": {
        "user": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Get current authenticated user.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/users/me`

<aside class="success">
Return a 200 status code with the current authenticated user.
</aside>

## Modify Current User

```json
{
    "message": null,
    "payload": {
        "user": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Modify current authenticated user.
This requests needs a JWT token to work.

### HTTP Request

`PUT https://api.sportsnconnect.com/users/me`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
first_name | String | First name of the user.
last_name | String | Last name of the user.
email | String | Email of the user.
birthday | String | Birthday of the user.
town | String | Town of the user.
country | String | Country of the user.
weight | String | Weight of the user.
height | String | Height of the user.
postal_code | String | Postal Code of the user.
phone | String | Phone of the user.
about | String | Profile's description of the user.
level_id | Integer | Sport Level of the user. 0: Beginner, 1: Good, 2: Very Good, 3: Expert
lat | String | Latitude of the user.
lng | String | Longitude of the user.
disciplines | String | Disciplines of the user. Format: "11,2,3"
avatar | File | Avatar of the user. This is a multipart file.
license | File | Sport License of the user. This is a multipart file.
medical_certif | File | Medical Certification of the user. This is a multipart file.

<aside class="success">
Return a 200 status code if the requested modification(s) succeded.
</aside>

## Get Current User Events

```json
{
    "message": null,
    "payload": {
        "events": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Get current authenticated user's events.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/users/me/events`

<aside class="success">
Return a 200 status code with the current authenticated user's events.
</aside>

## Get Current User Trainings

```json
{
    "message": null,
    "payload": {
        "trainings": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Get current authenticated user's trainings.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/users/me/trainings`

<aside class="success">
Return a 200 status code with the current authenticated user's trainings.
</aside>

## Get Current User closest Stores

```json
{
    "message": null,
    "payload": {
        "stores": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Get current authenticated user's closest stores.
This requests needs a JWT token to work.

### HTTP Request

`GET https://api.sportsnconnect.com/users/me/stores`

<aside class="success">
Return a 200 status code with the current authenticated user's closest stores.
</aside>

## Get User by Id

```json
{
    "message": null,
    "payload": {
        "user": {
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        }
    }
```

Returns requested user if the user exists.

### HTTP Request

`GET https://api.sportsnconnect.com/users/:userId`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
userId | Integer | Required. The id of the user to search.

<aside class="success">
Return a 200 status code with the user.
</aside>

## Get User Friends by Id

```json
{
    "message": null,
    "payload": {
        "friends": [{
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        },
        ...]
    }
```

Returns requested user's friends if the user exists.

### HTTP Request

`GET https://api.sportsnconnect.com/users/:userId/friends`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
userId | Integer | Required. The id of the user to search.

<aside class="success">
Return a 200 status code with a list of the user's friends.
</aside>

## Get User Teams by Id

```json
{
    "message": null,
    "payload": {
        "teams": [{
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        },
        ...]
    }
```

Returns requested user's teams if the user exists.

### HTTP Request

`GET https://api.sportsnconnect.com/users/:userId/teams`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
userId | Integer | Required. The id of the user to search.

<aside class="success">
Return a 200 status code with a list of the user's teams.
</aside>

## Get User Events by Id

```json
{
    "message": null,
    "payload": {
        "events": [{
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        },
        ...]
    }
```

Returns requested user's events if the user exists.

### HTTP Request

`GET https://api.sportsnconnect.com/users/:userId/events`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
userId | Integer | Required. The id of the user to search.

<aside class="success">
Return a 200 status code with a list of the user's events.
</aside>

## Get User Trainings by Id

```json
{
    "message": null,
    "payload": {
        "trainings": [{
            "id": 14400,
            "name": "Vincent Ducloup",
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "salt": null,
            "role_id": 2,
            "avatar": "avatar_url",
            "photo": "photo_url",
            "created": "2019-12-13T10:33:15.000Z",
            "last_login": "2019-12-13T10:33:15.000Z",
            "photo_count": 2,
            "friend_count": 1,
            "notification_count": 0,
            "friend_request_count": 0,
            "blog_count": 0,
            "topic_count": 0,
            "group_count": 0,
            "event_count": 0,
            "conversation_user_count": 41,
            "video_count": 0,
            "gender": "Male",
            "birthday": "1997-04-15",
            "active": 1,
            "confirmed": 1,
            "code": "",
            "notification_email": 1,
            "timezone": "Europe/Paris",
            "ip_address": "ip_address",
            "privacy": 1,
            "username": "",
            "about": "",
            "featured": 0,
            "lang": "",
            "hide_online": 0,
            "cover": "",
            "approved": 1,
            "is_social": 0,
            "has_active_subscription": 0,
            "receive_message_from_non_friend": 1,
            "send_email_when_send_message": 1,
            "request_friend_email": 1,
            "notification_setting": null,
            "profile_type_id": 1,
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "phone": "0666666666",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "disciplines": "11,1,2,3,4,6",
            "distance": 0,
            "level_id": 1,
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": 0,
            "training_count": 0,
            "team_count": 0,
            "address": "Rue de Rivoli",
            "city": "Paris",
            "state": "",
            "country": "France",
            "bike1_id": 0,
            "is_pro": 0,
            "social_avatar": "",
            "magasin": 0,
            "postal_code": 75001,
            "user_license": null
        },
        ...]
    }
```

Returns requested user's trainings if the user exists.

### HTTP Request

`GET https://api.sportsnconnect.com/users/:userId/trainings`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
userId | Integer | Required. The id of the user to search.

<aside class="success">
Return a 200 status code with a list of the user's trainings.
</aside>
# Authentication

## Login with email

> Success:

```json
{
    "message": null,
    "payload": {
        "user_id": "the_user_id",
        "access_token": "the_access_token"
    },
    "status": 200
}
```

> Error:

```json
{
    "message": "Ce compte n'existe pas.",
    "payload": null,
    "status": 400
}
```

This endpoint logs the user in and get his user id and his json web token (access token).

### HTTP Request

`POST https://api.sportsnconnect.com/auth/login`

### Query Parameters

Parameter | Description
--------- | -----------
email | User's email.
password | User's password.

<aside class="success">
If the call succeeds you'll get the user id and his access token (JWT).
</aside>

## Login with social (Facebook & Strava)

> Success:

```json
{
    "message": null,
    "payload": {
        "firstLogin": true
    },
    "status": 200
}
```

This endpoint logs in a user with a social media.

### HTTP Request

`POST https://api.sportsnconnect.com/auth/login`

### Query Parameters

Parameter | Type | Description
--------- | ---- | -----------
email | String | User's email
provider_uid | Int | The user id that comes from the provider (Facebook or Strava).
provider | String | The provider ("facebook" or "strava")
profilePictureURL | String | The user's profile picture get by the provider.
first_name | String | The user's first name get by the provider.
last_name | String | The user's last name get by the provider.

<aside class="notice">
If the user logs in for the first time, firstLogin will be true, if not it will be false.
</aside>

## Forgot password

This endpoint ask for an email to reset the password.

### HTTP Request

`POST https://api.sportsnconnect.com/auth/reset-password`

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
email | String | User's email where he wants to receive the reset password email.

<aside class="success">
Returns status code 200.
</aside>

## Register

```json
{
    "message": "User successfully registered.",
    "payload": {
        "user": {
            "role_id": "2",
            "photo_count": "0",
            "friend_count": "0",
            "notification_count": "0",
            "friend_request_count": "0",
            "blog_count": "0",
            "topic_count": "0",
            "group_count": "0",
            "event_count": "0",
            "conversation_user_count": "0",
            "video_count": "0",
            "active": "1",
            "confirmed": "1",
            "notification_email": "1",
            "privacy": "1",
            "featured": "0",
            "hide_online": "0",
            "approved": "0",
            "is_social": "0",
            "has_active_subscription": "0",
            "receive_message_from_non_friend": "1",
            "send_email_when_send_message": "1",
            "request_friend_email": "1",
            "profile_type_id": "1",
            "phone": "",
            "facebook_link": "",
            "twitter_handle": "",
            "instagram_handle": "",
            "strava_handle": "",
            "linkedin_handle": "",
            "distance": "0",
            "level_id": "1",
            "lat": "0.00000000",
            "lng": "0.00000000",
            "kilometer_count": "0",
            "training_count": "0",
            "team_count": "0",
            "state": "",
            "bike1_id": "0",
            "is_pro": "0",
            "social_avatar": "",
            "magasin": "0",
            "postal_code": null,
            "id": 14574,
            "email": "useremail@test.fr",
            "password": "the_user_password",
            "name": "Vincent Ducloup",
            "avatar": "avatar_url",
            "photo": "photo_url",
            "gender": "male",
            "first_name": "Vincent",
            "last_name": "Ducloup",
            "birthday": "2020-09-01",
            "address": "2 Rue du Moulin",
            "city": "OK",
            "country": "oui",
            "disciplines": "1,2",
            "code": "",
            "ip_address": "ip_address",
            "timezone": "",
            "username": "",
            "about": "",
            "lang": "",
            "cover": "",
            "created": "2020-01-13T21:26:02.000Z"
        },
        "access_token": "the_access_token"
    },
    "status": 200
}
```

> Error:

```json
{
    "message": "Email address already used.",
    "payload": null,
    "status": 400
}
```

Register the user.

<aside class="notice">
This request is a multipart form data request.
</aside>

### HTTP Request

`POST https://api.sportsnconnect.com/auth/register`

### URL Parameters

Parameter | Type | Description
--------- | ---- | -----------
email | String |
password | String |
avatar | File |
first_name | String |
last_name | String |
gender | String | 'male' or 'female'
birthday | String | Has to be UTC date.
address | String |
city | String |
country | String |
disciplines | [Int] | User's disciplines array.
license | File | User's license.
medical_certif | File | User's medical certificate.
---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

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

### URL Parameters

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

### URL Parameters

Parameter | Type | Description
--------- | ---- | -----------
Email | String | User's email where he wants to receive the reset password email.

<aside class="success">
Returns status code 200.
</aside>


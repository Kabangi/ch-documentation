# Users

## Register a new user
### HTTP Request
Remember to send access_token(client) along

`POST /users`

Parameter | Type | Description
---------- | ------- | --------
username | String | User username
password | String | User password
password_confirmation | String | Password confirmation same as password
firstName | String | User Firstname

## Account Verification
Upon registration the user gets an email with a link with a token to verify his/her email address
'GET /users/verification/email/token'

```shell
curl "/users/verification/email/token"
  -H "Authorization: access_token"
```
> The above command returns JSON structured like this:

```json

	{
	    "access_token": "igD3kqp7sN8aSZtPBBNLLrVcYe0zHAQk6xnUdwd5",
	    "token_type": "Bearer",
	    "expires_in": 3600
	}
```

## Login a user
`POST /login`

Response access_token that should then be used to make subsequent requests 

Parameter | Type | Description
---------- | ------- | --------
username | String | User username
password | String | User password
client_id | String | User Firstname
client_secret | String | User Firstname


```shell
curl "https://api.connecthealth.io/login"
  -H "Authorization: access_token"
```
> The above command returns JSON structured like this:

```json

	{
	    "access_token": "igD3kqp7sN8aSZtPBBNLLrVcYe0zHAQk6xnUdwd5",
	    "token_type": "Bearer",
	    "expires_in": 3600
	}
```

## Password Reset
`POST /password/send-reminder`

Parameter | Type | Description
---------- | ------- | --------
email | String | User email

`POST /password/reset`

Parameter | Type | Description
---------- | ------- | --------
email | String | User email
password | String | New User password
password_confirmation | String | New User password confirmation. Same as password
token | String | Reset token that was sent to user's email

## Changing Password
`POST /users/{id}/change-password`

## Updating User
`POST /users/{id}`


## Show User
`GET /users/{id}`

## Deleting User
`DELETE /users/{id}`

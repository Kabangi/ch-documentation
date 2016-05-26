#Appointments
## Register a new appointment
```shell
curl "/appointments"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /appointments`
Requires the access token to be that of an authenticated user

Parameters | Required | Description
---------- | ------- | ------------


## List Doctors

```shell
curl "/appointments"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": [
    ]
}
```

`GET /appointments`

## Show a single appointment
```shell
curl "/appointments/10"
  -H "Authorization: Bearer {access_token}"
```
```json
{
    "data": {
       
    }
}
```

`GET /appointments/{id}`

## Update appointment
```shell
curl "/appointments/1"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /appointments/{id}`
Requires the access token to be that of an authenticated user for either the admin or the appointment owner

Parameters | Required | Description
---------- | ------- | ------------

## Search for appointments
```shell
curl "/appointments/search?"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": {
       
    }
}
```

`GET /appointments/search?field=value&field2=value`

Parameters | Required | Description
---------- | ------- | ------------

## Delete appointment
```shell
curl "/appointments/{id}"
  -H "Authorization: Bearer {access_token}"
```
> Response:

```json
    {
        "message": "Event was deleted"
    }
```
`DELETE /appointments/{id}`

Requires the access token to be that of an authenticated user for either the admin or the appointment owner



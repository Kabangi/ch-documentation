#Schedules
## Register a new schedule
```shell
curl "/schedules"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /schedules`
Requires the access token to be that of an authenticated user

Parameters | Required | Description
---------- | ------- | ------------


## List Doctors

```shell
curl "/schedules"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": [
    ]
}
```

`GET /schedules`

## Show a single schedule
```shell
curl "/schedules/10"
  -H "Authorization: Bearer {access_token}"
```
```json
{
    "data": {
       
    }
}
```

`GET /schedules/{id}`

## Update schedule
```shell
curl "/schedules/1"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /schedules/{id}`
Requires the access token to be that of an authenticated user for either the admin or the schedule owner

Parameters | Required | Description
---------- | ------- | ------------

## Search for schedules
```shell
curl "/schedules/search?"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": {
       
    }
}
```

`GET /schedules/search?field=value&field2=value`

Parameters | Required | Description
---------- | ------- | ------------

## Delete schedule
```shell
curl "/schedules/{id}"
  -H "Authorization: Bearer {access_token}"
```
> Response:

```json
    {
        "message": "Event was deleted"
    }
```
`DELETE /schedules/{id}`

Requires the access token to be that of an authenticated user for either the admin or the schedule owner



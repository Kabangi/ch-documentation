#Practices
## Register a new practice
```shell
curl "/practices"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /practices`
Requires the access token to be that of an authenticated user

Parameters | Required | Description
---------- | ------- | ------------


## List Doctors

```shell
curl "/practices"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": [
    ]
}
```

`GET /practices`

## Show a single practice
```shell
curl "/practices/10"
  -H "Authorization: Bearer {access_token}"
```
```json
{
    "data": {
       
    }
}
```

`GET /practices/{id}`

## Update practice
```shell
curl "/practices/1"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /practices/{id}`
Requires the access token to be that of an authenticated user for either the admin or the practice owner

Parameters | Required | Description
---------- | ------- | ------------

## Search for practices
```shell
curl "/practices/search?"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": {
       
    }
}
```

`GET /practices/search?field=value&field2=value`

Parameters | Required | Description
---------- | ------- | ------------

## Delete practice
```shell
curl "/practices/{id}"
  -H "Authorization: Bearer {access_token}"
```
> Response:

```json
    {
        "message": "Event was deleted"
    }
```
`DELETE /practices/{id}`

Requires the access token to be that of an authenticated user for either the admin or the practice owner



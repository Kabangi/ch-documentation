#Doctors
## Register a new doctor
```shell
curl "/doctors"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /doctors`
Requires the access token to be that of an authenticated user

Parameters | Required | Description
---------- | ------- | ------------


## List Doctors

```shell
curl "/doctors"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": [
    ]
}
```

`GET /doctors`

## Show a single doctor
```shell
curl "/doctors/10"
  -H "Authorization: Bearer {access_token}"
```
```json
{
    "data": {
       
    }
}
```

`GET /doctors/{id}`

## Update doctor
```shell
curl "/doctors/1"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /doctors/{id}`
Requires the access token to be that of an authenticated user for either the admin or the doctor owner

Parameters | Required | Description
---------- | ------- | ------------

## Search for doctors
```shell
curl "/doctors/search?"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": {
       
    }
}
```

`GET /doctors/search?field=value&field2=value`

Parameters | Required | Description
---------- | ------- | ------------

## Delete doctor
```shell
curl "/doctors/{id}"
  -H "Authorization: Bearer {access_token}"
```
> Response:

```json
	{
    	"message": "Event was deleted"
	}
```
`DELETE /doctors/{id}`

Requires the access token to be that of an authenticated user for either the admin or the doctor owner



#Patients
## Register a new patient
```shell
curl "/patients"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /patients`
Requires the access token to be that of an authenticated user

Parameters | Required | Description
---------- | ------- | ------------


## List Doctors

```shell
curl "/patients"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": [
    ]
}
```

`GET /patients`

## Show a single patient
```shell
curl "/patients/10"
  -H "Authorization: Bearer {access_token}"
```
```json
{
    "data": {
       
    }
}
```

`GET /patients/{id}`

## Update patient
```shell
curl "/patients/1"
  -H "Authorization: Bearer {access_token}"
  -F 'name=name' \
```

```json
{
    "data": [
       
    ]
}
```
`POST /patients/{id}`
Requires the access token to be that of an authenticated user for either the admin or the patient owner

Parameters | Required | Description
---------- | ------- | ------------

## Search for patients
```shell
curl "/patients/search?"
  -H "Authorization: Bearer {access_token}"
```

```json
{
    "data": {
       
    }
}
```

`GET /patients/search?field=value&field2=value`

Parameters | Required | Description
---------- | ------- | ------------

## Delete patient
```shell
curl "/patients/{id}"
  -H "Authorization: Bearer {access_token}"
```
> Response:

```json
    {
        "message": "Event was deleted"
    }
```
`DELETE /patients/{id}`

Requires the access token to be that of an authenticated user for either the admin or the patient owner



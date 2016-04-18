#Sms

## Send a sms to a user
### HTTP Request
Remember to send access_token along

`POST /sms`

Parameter | Type | Description
---------- | ------- | --------
recipients | String or Array | Intended receipients
message | String | Message to user

```shell
curl "/sms"
  -H "Authorization: access_token"
```
> The above command returns JSON structured like this:

```json

	{
	    "message": "Message sent successfully"
	}
```
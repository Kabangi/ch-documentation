#Sms

## Send a sms to a user(s)

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

### HTTP Request
Remember to send access_token along
Use this end point to also send bulk messages and non bulk messages
`POST /sms`

Sending a single message to multiple users or one

Parameter | Type | Description
---------- | ------- | --------
recipients | String or Array | Intended receipients or a single receipient as string
message | String | Message to user

Sending messages each user with his own custom message

Parameter | Type | Description
---------- | ------- | --------
sms | Object i.e {number:value,message:value} |  Messages payload with equivalent reciepient

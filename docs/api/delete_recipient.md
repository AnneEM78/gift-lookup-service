# Delete recipient

Delete a recipient from the recipient list.

## URL

```shell

DELETE {server_url}/recipients/<id>
```

## Request headers

This request does not use any authorization. The endpoint is available to all users and applications.

| Header name | Description | Required | Values |
| -------------- | ------ | ------------ |------------ |
| Recipient | The recipient to be deleted. | Optional | application/json. Default value. |

## Request body

None

## Sample request

The DELETE request should look like this.

```js
{server_url}/recipients/<id>
```

It uses the **DELETE** method and returns a the response shown in the **Return body**.

## Return body

None

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 201 | Deleted | Recipient deleted successfully. |
| 500 | Internal server Error | Invalid JSON. |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

## Related information

* [Handling errors](handling_errors)

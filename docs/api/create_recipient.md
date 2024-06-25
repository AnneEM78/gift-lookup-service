# Create recipient

Creates a `recipient` for a gift list.
The request body contains the new recipient details.
You must specify the required properties for the recipient.

## URL

```shell
{POST}{server_url}/recipients/
```

## Request headers

This request does not use any authorization. The endpoint is available to all users and applications.

| Header name | Description | Required | Values |
| -------------- | ------ | ------------ |------------ |
| Content-Type | The format of the data to be posted. | Optional | application/json. Default value.  |
| Accept | The format of the data to be returned. | Optional | application/json. Default value. |

## Request body

In the request body, specify a JSON representation of the recipient object. The following table lists the properties that are required when you create a recipient.

| Property | Description | Type | Required | Notes |
| -------------- | ------ | ------------ |------------ |------------ |
| last_name | The recipient's last name. | String | Required |   |
| first_name | The recipient's first name. | String | Required |  |
| date_of_birth | The recipient's birthdate. | String | Required | MMDDYYYY format. |

## Sample request

The POST body should look something like this. You can change the values of each property as you’d like.

```js
[
    {
      "last_name": "Vaz",
      "first_name": "Elizabeth",
      "date_of_birth": "2020-04-14"
    }
]
```

## Return body

The following example shows the response. Note that the name should be the same as what you used in your **Request body** and the response should include the new recipient's id. The recipient's id is automatically generated when the recipient is created.

```js
[
    {
      "last_name": "Vaz",
      "first_name": "Elizabeth",
      "date_of_birth": "2020-04-14",
      "id": 1
    }
]
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 201 | Created | User data created successfully. |
| 500 | Internal server Error | Invalid JSON. |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

## Related information

- [Handling errors](api/handling_errors.md)

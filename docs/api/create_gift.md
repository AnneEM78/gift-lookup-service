# Create gift

Creates a [`gift`](gift) for a gift list.
The request body contains the gift details.
You must specify the required properties for the gift.

## URL

```shell

{POST}{server_url}/gifts/
```

## Request headers

This request does not use any authorization. The endpoint is available to all users and applications.

| Header name | Description | Required | Values |
| -------------- | ------ | ------------ |------------ |
| Content-Type | The format of the data to be posted. | Optional | application/json. Default value.  |
| Accept | The format of the data to be returned. | Optional | application/json. Default value. |

## Request body

In the request body, specify a JSON representation of the [`gift`](gift) object. The following table lists the properties that are required when you create a gift.

| Property | Description | Type | Required | Notes |
| -------------- | ------ | ------------ |------------ |------------ |
| user_id | The recipient's id. | string | Required |   |
| title | The name of the gift. | string | Required |  |
| date_gifted | The date the gift was given. | string | Required | MMDDYYYY format. |

## Sample request

The POST body should look something like this. You can change the values of each property as you’d like.

```js
[
    {
      {
      "user_id": 1,
      "title": "Gabby's Dollhouse",
      "date_gifted": "2024-02-20",         
      }
    }
]
```

## Return body

The following example shows the response. Note that the name should be the same as what you used in your **Request body** and the response should include the new gift's id. The gift's id is automatically generated when the gift is created.

```js
[
    {
      "user_id": 1,
      "title": "Gabby's Dollhouse",
      "date_gifted": "2024-02-20",
      "gift_id": 1
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

* [Handling errors](api/handling-errors)

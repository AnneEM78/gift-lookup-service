# Get recipients by birthdate

Returns an array of  [`recipient`](recipient) objects that contains only the birthdate specified by the `date_of_birth` parameter, if it exists.

## URL

```shell
{server_url}/recipients/{date_of_birth}
```

## Params

| Parameter name | Type | Description |
| -------------- | ------ | ------------ |
| `date_of_birth` | number | The record birthdate of the user to return |

## Request headers

None

## Request body

None

## Return body

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `date_of_birth` | String | The recipient birthdate |

Sample task response

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
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified record not found |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

## Related information

* [Handling errors](handling_errors)

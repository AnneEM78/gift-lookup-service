# Get recipients by first name

Returns an array of `recipient` objects that contains only the name specified by the `first_name` parameter, if it exists.

## URL

```shell
{server_url}/users?first_name={first name to find}
```

## Params

| Parameter name | Type | Description |
| -------------- | ------ | ------------ |
| `first_name` | String | The first name of the user to return |

## Request headers

None

## Request body

None

## Return body

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `first_name` | String | The recipient's first name |

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

* [Handling errors](handling_errors.md)

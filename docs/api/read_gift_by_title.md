# Get gift by title

Returns an array of `gift` objects that contains only the gift specified by the `title` parameter, if it exists.

## URL

```shell
{server_url}/gifts/{title}
```

## Params

| Parameter name | Type | Description |
| -------------- | ------ | ------------ |
| `title` | String | The name of the gift |

## Request headers

None

## Request body

None

## Return body

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `title` | String | The name of the gift |

Sample task response

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
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified record not found |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

## Related information

- [Handling errors](api/handling_errors.md)

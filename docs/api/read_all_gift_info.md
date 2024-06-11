# Get all gift info

Returns an array of [`gift`](gift) objects entered into the service with all related information.

## URL

```shell
{server_url}/gifts
```

## Params

None

## Request headers

None

## Request body

None

## Return body

```js

"gifts": [
    {
      "user_id": 1,
      "title": "Gabby's Dollhouse",
      "date_gifted": "2024-02-20",
      "gift_id": 1
    },
    {
      "user_id": 1,
      "title": "Melissa & Doug toy piano",
      "date_gifted": "2023-04-05",
      "gift_id": 2
    },
    {
      "user_id": 2,
      "title": "Fiskars hedge shears",
      "date_gifted": "2021-03-09",
      "gift_id": 3
    },
    {
      "user_id": 3,
      "title": "toy fire truck",
      "date_gifted": "2022-05-11",
      "gift_id": 4
    },
    {
      "user_id": 4,
      "title": "Madewell tote bag",
      "date_gifted": "2022-05-11",
      "gift_id": 5
    }
  ]
  ```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

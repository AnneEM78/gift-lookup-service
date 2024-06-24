# Quickstart guide

## At a glance

This quickstart guide walks you through setting everything up in order to start using the Giftrackr service, which records gifts and recipients by name, including recipients' birthdates, allowing users of the service to organize what birthday gifts they've given and to whom, preventing duplicate gifts.

## How to use the Giftrackr service

To build your API call, you must have the following components:

* **A host.**  The {server_url} depends on users' installation of the service in their development environment. The **server_url** variable is typically set to `http://localhost:3000`.
* **Authorization.**  Requests do not use any authorization. All endpoints are available to all users and applications.
* **A request.**  The REST API enables CRUD operations via HTTP requests on database resources (`GET`, `POST`, `PUT`, `PATCH`, and `DELETE` methods). Request and response bodies are encoded as JSON.

### Supported endpoints

| HTTP Method | Endpoint |
| :--------------: | :--------------: |
| POST | [Create a recipient](api/create_recipient.md) |
| POST | [Create a gift](api/create_gift.md) |
| DELETE | [Delete gift](api/delete_gift.md) |
| DELETE | [Delete recipient](api/delete_recipient.md) |
| PATCH | [Update gift](api/update_gift.md) (coming soon) |
| PATCH | [Update recipient](api/update_recipient.md) (coming soon) |
| GET | [Get all gift info](api/read_all_gift_info.md) |
| GET | [Get recipients by birthdate](api/read_recipient_by_birthdate.md) |
| GET | [Get recipients by first name](api/read_recipient_by_first_name.md) |

## Make your first API call – *List all gifts*

```bash
curl http://localhost:3000/gifts
```

If the call was successful, the response you receive will be a list of gifts as you see in this example:

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
}
```

## Next steps

Follow these tutorials to perform common tasks in Giftrackr.

* [Add a recipient](tutorials/add_a_recipient.md)
* [Add a gift](tutorials/add_a_gift.md)

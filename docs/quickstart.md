# Quickstart guide

## At a glance

TBD

## Setting up

TBD

## How to use the Giftrackr service

To build your API call, you must have the following components:

* **A host.**  The {base_url} depends on users' installation of the service in their development environment. The **base_url** variable is typically set to `http://localhost:3000`.
* **Authorization.**  Requests do not use any authorization. All endpoints are available to all users and applications.
* **A request.**  The REST API enables CRUD operations via HTTP requests on database resources (`GET`, `POST`, `PUT`, `PATCH`, and `DELETE` methods). Request and response bodies are encoded as JSON.

### Supported endpoints

| HTTP Method | Endpoint |
| :--------------: | :--------------: |
| GET | --- |
| GET | --- |
| GET | --- |
| POST | --- |
| PUT |  --- |
| PATCH |  --- |
| PATCH |  --- |
| GET |  --- |
| CREATE |  --- |
| PATCH | --- |

## Make your first API call – *List all tasks*

```bash
curl http://localhost:3000/tasks
```

If the call was successful, the response you receive will be a list of gifts as you see in this example:

```js

  


---

## Next steps


# Update a recipient with PATCH

Use `PATCH` to update a recipient when you want to change only some of the information related to that recipient. You must supply the recipient `id` in both the request endpoint and the request body.

## Endpoint

The endpoint for using `PATCH` to update a recipient is:

{server_url}/recipients/{id}

```json

## Properties

The following example contains a request body for a `PATCH` request.

```json
{
}
```

## Descriptions

The following table defines properties in the request body.

| Property name | Type   | Description                                                                                                                                                 |

## Operations

When you use `PATCH` to update a recipient, you can:

* **Update an entire recipient** — Replace the entire request body.
* **Update part of a recipient** — Only replace the fields to update; omit the others.

> ℹ️ recipient `id` is required in both scenarios and must match in both the endpoint and the request body. For example, if you change the `id` in only the request body, the service returns a `200 OK`, but does not update the recipient.

## Examples

Use the following examples when sending `PATCH` requests to the Giftrackr service.

### cURL

```bash
curl 
}'
```

### Complete recipient body

```json
{
  
}
```

### Partial recipient body

```json
{
  
}
```

## Related information

* [Handling errors](handling_errors.md)

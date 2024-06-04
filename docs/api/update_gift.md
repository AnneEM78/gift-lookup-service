# Update a gift with PATCH

Use `PATCH` to update a gift when you want to change only some of the information related to that gift. You must supply the gift `id` in both the request endpoint and the request body. 

## Endpoint

The endpoint for using `PATCH` to update a gift is:

```
{server_url}/gifts/{id}
```

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

When you use `PATCH` to update a gift, you can:

* **Update an entire gift** — Replace the entire request body.
* **Update part of a gift** — Only replace the fields to update; omit the others. 

> ℹ️ Gift `id` is required in both scenarios and must match in both the endpoint and the request body. For example, if you change the `id` in only the request body, the service returns a `200 OK`, but does not update the gift. 

## Examples

Use the following examples when sending `PATCH` requests to the Giftrackr service.

### cURL

```bash
curl 
}'
```

### Complete gift body

```json
{
  
}
```
### Partial gift body

```json
{
  
}
```
## Related information

* [Handling errors](handling_errors.md)
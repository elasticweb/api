# Create a DNS entry

    POST api/dns/entry/:domain_name

## Description

Create a DNS entry for the domain.

## Parameters

- **type** _(required)_ — DNS entry type: A, TXT, MX, CNAME.
- **name** _(required)_ — DNS entry name. Example: www.
- **value** _(required)_ — DNS entry value: Example: test.com.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — The domain not belong to you | Validation Failed.
- **404 Not Found** — The domain name is not valid.
- **200 OK** — DNS entry created.

***

## Example response

```json
{
  "status":true,
  "message":"DNS entry created."
}
```

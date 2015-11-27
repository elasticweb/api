# Remove the DNS entry

    DELETE api/dns/entry/:dns_id

## Description

Remove the DNS entry by the DNS ID.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — The domain not belong to you.
- **404 Not Found** — DNS entry not found.
- **200 OK** — DNS entry deleted.

***

## Example response

```json
{
  "status":true,
  "message":"DNS entry deleted."
}
```

# Delete domain alias

    DELETE api/alias/entry/:alias_name

## Description

Delete a domain alias.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — Alias not found.
- **200 OK** — Domain alias deleted.

***

## Example response

```json
{
  "status":true,
  "message":"Alias deleted."
}
```

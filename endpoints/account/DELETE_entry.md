# Delete account

    DELETE api/account/entry/:id

## Description

Delete node.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — Account not found.

***

## Example response

```json
{
  "status":true,
  "message":"Account deleted."
}
```

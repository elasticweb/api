# Create new database

    POST api/database/entry/:account_id

## Description

Create new database.

## Parameters

- **name** _(required)_ — Database name.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.
- **404 Not Found** — Account not found.
- **200 OK** — Database created.

***

## Example response

```json
{
  "status":true,
  "message":"Database created.",
  "data": [
    {
      "id":1
    }
  ]
}
```

# Delete database user

    DELETE api/database_user/entry/:account_id/:db_user_name

## Description

Delete a database user.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.
- **404 Not Found** — Account or database user not found.
- **200 OK** — Database user deleted.

***

## Example response

```json
{
  "status":true,
  "message":"Database user deleted."
}
```

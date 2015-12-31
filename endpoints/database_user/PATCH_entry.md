# Edit database user.

    PATCH api/database_user/entry/:account_id/:db_user_name

## Description

Edit password and databases[] for database user.

## Parameters

- **password** — Database user password.
- **databases[]** _(required)_ — List of databases ID. ( See method: api/database/list/:account_id ).

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Problems parsing JSON | Validation Failed.
- **404 Not Found** — Account not found | Database user not found.
- **200 OK** — Database user updated.

***

## Example response

```json
{
  "status":true,
  "message":"Database user updated."
}
```

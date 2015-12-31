# Information about database user.

    GET api/database_user/entry/:account_id/:db_user_name

## Description

Get complete information about the database user.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — Account not found | Database user not found.

***

## Example response

```json
{
  "status":true,
  "data":{
    "id":"1",
    "name":"main",
    "account_id":"1",
    "server_id":"3",
    "databases":["99"],
    "created":"1450270232"
  }
}
```

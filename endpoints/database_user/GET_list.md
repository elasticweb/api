# The list of database users.

    GET api/database_user/list/:account_id

## Description

The list of database users for a account.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — Account not found.

***

## Example response

```json
{
  "status":true,
  "data":[
    {
      "id":"1",
      "name":"main",
      "account_id":"1",
      "server_id":"3",
      "databases":["99"],
      "created":"1450270232"
    },
    {
      "id":"2",
      "name":"main1",
      "account_id":"1",
      "server_id":"3",
      "databases":["100", "101"],
      "created":"1450270219"
    }
  ]
}
```

# Create new database user

    POST api/database_user/entry/:account_id

## Description

Create new database user.

## Parameters

- **name** _(required)_ — Database user name.
- **password** _(required)_ — Database user password.
- **databases[]** _(required)_ — List databases ID. ( see api/database/list/:account_id )

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.
- **404 Not Found** — Account not found.
- **200 OK** — Database user created.

***

## Example request

```
"name" => "test"
"password" => "hytiOntHEtio"
"databases[0]" => "1122"
"databases[1]" => "1123"
```

## Example response

```json
{
  "status":true,
  "message":"Database user created."
  }
}
```

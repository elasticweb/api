# Create new account

    POST api/account/entry

## Description

Create new user hosting-account.

## Parameters

- **server** _(required)_ — Server ID. See method ( GET api/account/list ).
- **domain** — Domain name without http and slash.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.

***

## Example response

```json
{
  "status":true,
  "message":"Account created.",
  "account":{
    "id":120,
    "status":1,
    "ip_address":"176.31.116.184",
    "server_host":"yellow.elastictech.org",
    "server_id":3
   }
  }
}
```

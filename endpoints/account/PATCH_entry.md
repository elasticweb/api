# Edit account

    PATCH api/account/entry/:id

## Description

Edit node.

## Parameters

- **status** _(required)_ — Account status: 1 - Enabled, 0 - Disabled.
- **password** — Password for general SSH and FTP accounts.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Problems parsing JSON | Validation Failed.
- **404 Not Found** — Account not found.

***

## Example response

```json
{
  "status":true,
  "message":"Account updated.",
  "account":{
    "id":120,
    "status":1,
    "ip_address":"176.31.116.184",
    "server_host":"yellow.elastictech.org",
    "server_id":3
  }
}
```

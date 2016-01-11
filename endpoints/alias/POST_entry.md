# Create new domain alias

    POST api/alias/entry/:account_id

## Description

Create new domain alias.

## Parameters

- **name** _(required)_ — Domain name.
- **parent_domain** _(required)_ — Parent domain name for alias.
- **error_log** — Error log status: 1 - Enabled, 0 - Disabled.
- **access_log** — Access log status: 1 - Enabled, 0 - Disabled.
- **mx_records** _(required)_ — MX record template: main,google,yandex,mail.ru.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.
- **404 Not Found** — Account not found.
- **200 OK** — Alias created.

***

## Example response

```json
{
  "status":true,
  "message":"Alias created."
}
```

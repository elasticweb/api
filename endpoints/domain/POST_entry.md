# Create new domain

    POST api/domain/entry/:account_id

## Description

Create new domain.

## Parameters

- **name** _(required)_ — Domain name.
- **error_log** — Error log status: 1 - Enabled, 0 - Disabled.
- **access_log** — Access log status: 1 - Enabled, 0 - Disabled.
- **wildcard** — Wildcard status: 1 - Enabled, 0 - Disabled.
- **mx_records** _(required)_ — MX record template: main,google,yandex,mail.ru.
- **nginx_id** _(required)_ — Nginx ID for domain. ( GET api/domain/api/domain/nginx_configurations )

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.
- **404 Not Found** — Account not found.
- **200 OK** — Domain created.

***

## Example response

```json
{
  "status":true,
  "message":"Domain created."
}
```

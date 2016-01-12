# Edit cron tasks for node

    PATCH api/account/cron/:id

## Description

Edit cron tasks for node.

## Parameters

- **tasks** — Cron tasks.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Problems parsing JSON.
- **404 Not Found** — Account not found.

***

## Example response

```json
{
  "status":true,
  "message":"Cron updated.",
  "data":"15 14 1 * * echo 1"
}
```

# Database list

    GET api/database/list/:account_id

## Description

Returns information about database for hosting-account.

## Errors
All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Not passed account_id. 
- **404 Not Found** — No databases.

***

## Example response

```json
{
  "status": true,
  "data": [
    {
      "id": 777,
      "name": "test",
      "created": 1448739395
    }
  ],
  "references": {
    "account": {
      "id": 403,
      "status": true,
      "server_id": 3,
      "server_host": "yellow.elastictech.org"
    }
  }
}
```

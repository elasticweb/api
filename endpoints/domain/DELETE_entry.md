# Delete domain

    DELETE api/domain/entry/:domain_name

## Description

Delete a domain.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Problems parsing JSON | Validation Failed.
- **404 Not Found** — Domain not found.
- **200 OK** — Domain deleted.

***

## Example response

```json
{
  "status":true,
  "message":"Domain deleted."
}
```

# Information about DNS records

    GET api/dns/entry/:dns_id

## Description

Get complete information about the DNS records.

## Errors
All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Domain does not belong to you.
- **404 Not Found** — DNS entry was not found.

***

## Example response

```json
{
  "status":true,
  "data":{
    "id":1,
    "name":"mx",
    "type":"A",
    "value":"176.31.116.184"
  }
}
```

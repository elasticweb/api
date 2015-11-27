# The list of DNS records

    GET api/dns/list/:domain_name

## Description

The list of DNS records for a domain.

## Errors
All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Not passed domain_name.
- **404 Not Found** — Domain not found.

***

## Example response

```json
{
  "status":true,
  "data":[
    {
      "id":1
      "name":"mx",
      "type":"A",
      "value":"176.31.116.184"
    },
    {
      "id":2
      "name":"www",
      "type":"CNAME",
      "value":"test.com"
    }
  ]
}
```

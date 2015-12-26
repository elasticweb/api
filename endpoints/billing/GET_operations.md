# Types of operations

    GET api/billing/operations/:type_name

## Description

Returns a list of operations by type.

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — Operation type not found.

***

## Example response

```json
{
  "status":true,
  "data":[
    {
      "id":20000,
      "account_id":1,
      "extra":{
        "web_in":"0",
        "web_out":"0",
        "db_in":"0",
        "db_out":"0",
        "cpu":"0",
        "db_cpu":"0",
        "memory":"0",
        "io_read":"0",
        "io_write":"0",
        "disk_file":"0.0005",
        "disk_email":"0",
        "disk_db":"0",
        "total":0.0005
      },
      "timestamp":1450815002
    }
  ],
  "references":{
    "types":{
      "daily_invoice":"Daily invoice for node.",
      "balance":"Balance refill.",
      "partner":"Partner remuneration.",
      "service_invoice":"Service daily invoice."
    }
  },
  "pager":{
    "total":158,
    "per_page":50,
    "current_page":1,
    "next_page_url":"https:\/\/elasticweb.org\/api\/billing\/operations\/daily_invoice?page=2",
    "prev_page_url":null
  }
}
```

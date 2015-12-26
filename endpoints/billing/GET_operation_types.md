# Types of operations

    GET api/billing/operation_types

## Description

Returns information about the types of billing operations.

***

## Example response

```json
{
  "status":true,
  "data":{
    "daily_invoice":"Daily invoice for node.",
    "balance":"Balance refill.",
    "partner":"Partner remuneration.",
    "service_invoice":"Service daily invoice."
  }
}
```

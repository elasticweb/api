# Account

    GET api/account/list

## Description

Returns information about user accounts.

## Errors
All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **404 Not Found** — This user has no previously created accounts.

***

## Example response

```json
{
  "status":true,
  "data":[
    {
      "id":999,
      "status":1,
      "ip_address":"176.31.116.184",
      "server_name":"Yellow",
      "server_id":3
    }
  ],
  "references":{
    "servers":[
      {
        "server_id":3,
        "name":"Yellow",
        "host":"yellow.elastictech.org",
        "ip_address":"176.31.116.184",
        "information":"France. PHP 5.6 \/ MySQL (MariaDB 10) :: 96 GB RAM | 2x Intel Xeon E5606"
      }
    ]
  }
}
```

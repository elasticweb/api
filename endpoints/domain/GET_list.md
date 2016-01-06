# Domains list

    GET api/domain/list/:account_id

## Description

Returns information about domains for hosting-account.

## Errors
All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Not passed account_id. 
- **404 Not Found** — Account not have domains.

***

## Example response

```json
{
  "status":true,
  "data":[
    {
      "id":1
      "server_id":3,
      "name":"test.yellow.elastictech.org",
      "error_log":0,
      "access_log":0,
      "mx_records":"main",
      "nginx_id":0
    },
    {
      "id":2,
      "server_id":3,
      "name":"test1.yellow.elastictech.org",
      "error_log":0,
      "access_log":0,
      "mx_records":"main",
      "nginx_id":0
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
    ],
    "nginx_configurations":{
      "1":"Default config",
      "2":"Drupal 7",
      "4":"CMS Made Simple",
      "5":"Joomla 2, 3",
      "6":"Kohana",
      "9":"phpBB3",
      "11":"Symfony",
      "12":"Wordpress 4",
      "13":"Zend Framework",
      "15":"ZenCart 1.5",
      "16":"Laravel",
      "17":"Octobercms",
      "18":"MaxSite CMS",
      "19":"Asgard CMS",
      "20":"Codeigniter",
      "21":"OpenCart 1.5",
      "22":"MediaWiki",
      "23":"KodiCMS"
    }
  }
}
```

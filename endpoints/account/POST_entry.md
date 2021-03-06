# Create new account

    POST api/account/entry

## Description

Create new node. Access for SSH / SFTP authorization will be:

```
host: yellow.elastictech.org
username: u120
password: mOH9gTFYXkp9
```

See example response.

## Parameters

- **server** _(required)_ — Server ID. See method ( GET api/account/list ).
- **domain** _(optional)_ — Domain name without http and slash.
- **nginx_id** _(optional)_ — Nginx ID for domain. ( GET api/domain/api/domain/nginx_configurations )

## Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'message' keys describing the source of error.

- **400 Bad Request** — Validation Failed.

***

## Example response

```json
{
  "status":true,
  "message":"Account created.",
  "account":{
    "id":120,
    "status":1,
    "ip_address":"176.31.116.184",
    "server_host":"yellow.elastictech.org",
    "server_id":3,
    "password":"mOH9gTFYXkp9"
  }
}
```

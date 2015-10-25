# Elasticweb API

## Sandbox

You can edit status Sandbox on page http://elasticweb.org/user/api.

## Potential errors

* **200 OK**: _Successful API request._
* **201 Created**: _The request has been fulfilled and a new resource has been created._
* **400 Bad Request**: _The request cannot be fulfilled due to bad syntax._
* **401 Unauthorized**: _Authentication is required and has not been provided or has failed._
* **404 Not Found**: _The requested resource could not be found but could be available again in the future._

## Endpoints

#### Account

- **[<code>GET</code> api/account/list](https://github.com/elasticweb/api/blob/master/endpoints/account/GET_list.md)**
- **[<code>POST</code> api/account/entry](https://github.com/elasticweb/api/blob/master/endpoints/account/POST_entry.md)**
- **[<code>PATCH</code> api/account/entry/:id](https://github.com/elasticweb/api/blob/master/endpoints/account/PATCH_entry.md)**
- **[<code>DELETE</code> api/account/entry/:id](https://github.com/elasticweb/api/blob/master/endpoints/account/DELETE_entry.md)**

#### Domain

- **[<code>GET</code> api/domain/api/domain/nginx_configurations](https://github.com/elasticweb/api/blob/master/endpoints/domain/GET_nginx_configurations.md)**

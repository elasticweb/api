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

#### User

- **[<code>GET</code> api/user/me](https://github.com/elasticweb/api/blob/master/endpoints/user/GET_me.md)**

#### Account

- **[<code>GET</code> api/account/list](https://github.com/elasticweb/api/blob/master/endpoints/account/GET_list.md)**
- **[<code>POST</code> api/account/entry](https://github.com/elasticweb/api/blob/master/endpoints/account/POST_entry.md)**
- **[<code>PATCH</code> api/account/entry/:id](https://github.com/elasticweb/api/blob/master/endpoints/account/PATCH_entry.md)**
- **[<code>DELETE</code> api/account/entry/:id](https://github.com/elasticweb/api/blob/master/endpoints/account/DELETE_entry.md)**

#### Server

- **[<code>GET</code> api/server/list](https://github.com/elasticweb/api/blob/master/endpoints/server/GET_list.md)**

#### Alias

- **[<code>GET</code> api/alias/list/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/alias/GET_list.md)**
- **[<code>POST</code> api/alias/entry/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/alias/POST_entry.md)**
- **[<code>PATCH</code> api/alias/entry/:alias_name](https://github.com/elasticweb/api/blob/master/endpoints/alias/PATCH_entry.md)**
- **[<code>DELETE</code> api/alias/entry/:alias_name](https://github.com/elasticweb/api/blob/master/endpoints/alias/DELETE_entry.md)**

#### Domain

- **[<code>GET</code> api/domain/list/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/domain/GET_list.md)**
- **[<code>GET</code> api/domain/nginx_configurations](https://github.com/elasticweb/api/blob/master/endpoints/domain/GET_nginx_configurations.md)**
- **[<code>POST</code> api/domain/entry/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/domain/POST_entry.md)**
- **[<code>PATCH</code> api/domain/entry/:domain_name](https://github.com/elasticweb/api/blob/master/endpoints/domain/PATCH_entry.md)**
- **[<code>DELETE</code> api/domain/entry/:domain_name](https://github.com/elasticweb/api/blob/master/endpoints/domain/DELETE_entry.md)**

#### DNS

- **[<code>GET</code> api/dns/list/:domain_name](https://github.com/elasticweb/api/blob/master/endpoints/dns/GET_list.md)**
- **[<code>GET</code> api/dns/entry/:dns_id](https://github.com/elasticweb/api/blob/master/endpoints/dns/GET_entry.md)**
- **[<code>POST</code> api/dns/entry/:domain_name](https://github.com/elasticweb/api/blob/master/endpoints/dns/POST_entry.md)**
- **[<code>DELETE</code> api/dns/entry/:dns_id](https://github.com/elasticweb/api/blob/master/endpoints/dns/DELETE_entry.md)**

#### Database

- **[<code>GET</code> api/database/list/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/database/GET_list.md)**
- **[<code>POST</code> api/database/entry/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/database/POST_entry.md)**
- **[<code>DELETE</code> api/database/entry/:account_id/:db_name](https://github.com/elasticweb/api/blob/master/endpoints/database/DELETE_entry.md)**

#### Database user

- **[<code>GET</code> api/database_user/list/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/database_user/GET_list.md)**
- **[<code>GET</code> api/database_user/entry/:account_id/:db_user_name](https://github.com/elasticweb/api/blob/master/endpoints/database_user/GET_entry.md)**
- **[<code>POST</code> api/database_user/entry/:account_id](https://github.com/elasticweb/api/blob/master/endpoints/database_user/POST_entry.md)**
- **[<code>PATCH</code> api/database_user/entry/:account_id/:db_user_name](https://github.com/elasticweb/api/blob/master/endpoints/database_user/PATCH_entry.md)**
- **[<code>DELETE</code> api/database_user/entry/:account_id/:db_user_name](https://github.com/elasticweb/api/blob/master/endpoints/database_user/DELETE_entry.md)**

#### Billing

- **[<code>GET</code> api/billing/operation_types](https://github.com/elasticweb/api/blob/master/endpoints/billing/GET_operation_types.md)**
- **[<code>GET</code> api/billing/operations/:type_name](https://github.com/elasticweb/api/blob/master/endpoints/billing/GET_operations.md)**

## Examples

- **[PHP](https://github.com/elasticweb/api/blob/master/examples/php.md)**

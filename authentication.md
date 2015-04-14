# General information about authentication

Authentication is done by using `hapi-auth-cookie`. There is no encryption from client to server when sending credetials for login. Therefor we definitly need tls support.



# Board

### Routes
The following routes are defined

####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/logout   | kills the current session, user will be logged out    | TODO: currently string | statusCode: 401 | 

####POST

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/login   | tries to log a user in | statusCode: 200 | statusCode: 401, 401, 400 | 

### Dummy Json Results

#### Post

```
{
  "username": "tiweiss",
  "password": "secret"
}
```

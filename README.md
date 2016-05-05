# ConoHa-API
ConoHa API Documantation for Postman,

[ConoHa API Documantation](https://www.conoha.jp/docs/)

[POSTMAN GITHUB](https://github.com/postmanlabs/postman-app-support)

## Usage

- 1.Please install POSTMAN
- 2.Please import to JSON
- 3.Set Your Parameters
- 4.GET Token

### 1.install POSTMAN

[POSTMAN](http://www.getpostman.com/)

### 2.Import JSON

[environment](https://raw.githubusercontent.com/tacyan/ConoHa-API/master/Conoha.postman_environment)

[collections](https://github.com/tacyan/ConoHa-API/blob/master/Conoha.json.postman_collection)

### 3.Set Parameters

|Parameter|	Value|	Style	|Description|
|:-:|:-:|:-:|:-:|
|username	|ユーザー名|	plain|	ユーザ名|
|password	|ユーザーパスワード|	plain	|ユーザパスワード|
|tenantId (Optional)|	Tenant ID	|plain	|テナントID|

### 4.GET Token

Identity
#### POST /v2.0/tokens

```
{ "auth": 
  { "passwordCredentials": 
    { "username": "{{username}}", 
      "password": "{{password}}"
    },
    "tenantId": "{{tenant_id}}"
  }
}
```

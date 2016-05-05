# ConoHa-API
ConoHa API Documantation for Postman,

<a href="https://www.getpostman.com/"><img src="https://raw.githubusercontent.com/postmanlabs/postmanlabs.github.io/develop/global-artefacts/postman-logo%2Btext-320x132.png" /></a><br />

[ConoHa API Documantation](https://www.conoha.jp/docs/)

## Usage

- 1.Please install POSTMAN
- 2.Please import to JSON
- 3.Set Your Parameters
- 4.GET Token

### 1.install POSTMAN

[POSTMAN](http://www.getpostman.com/)

[POSTMAN GITHUB](https://github.com/postmanlabs/postman-app-support)

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

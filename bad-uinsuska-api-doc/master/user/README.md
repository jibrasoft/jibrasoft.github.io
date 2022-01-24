# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
User API Spec

## Authentication
No authentication needed to use this API

## Get User
Request :
- Method : GET
- Endpoint : `/api/user/{username}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "username" : "string",
         "level" : "string",
         "flag" : "integer|default:1"
    }
}
```

## List User
Request :
- Method : GET
- Endpoint : `/api/user`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "username" : "string",
             "level" : "string",
             "flag" : "integer|default:1"
        },
        {
             "username" : "string",
             "level" : "string",
             "flag" : "integer|default:1"
        }
    ]
}
```

## Authenticate User
Request :
- Method : POST
- Endpoint : `/api/user`
- Header :
    - Content-Type: application/json
    - Accept: application/json
- Body  :

```json 
{
    "username" : "string",
    "password" : "string"
}
```
    
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
          "username" : "string",
          "level" : "string",
          "flag" : "integer|default:1",
          "api_key" : "string"
    }
}
```
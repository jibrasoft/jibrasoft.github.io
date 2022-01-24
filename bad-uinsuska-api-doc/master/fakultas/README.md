# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Fakultas API Spec

## Authentication
No authentication needed to use this API

## Get Fakultas
Request :
- Method : GET
- Endpoint : `/api/fakultas/{id}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "id" : "string",
         "nama_fakultas" : "string",
         "akreditasi" : "string"
    }
}
```

## List Fakultas
Request :
- Method : GET
- Endpoint : `/api/fakultas`
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
            "id" : "string",
            "nama_fakultas" : "string",
            "akreditasi" : "string"
        },
        {
            "id" : "string",
            "nama_fakultas" : "string",
            "akreditasi" : "string"
        }
    ]
}
```

## Get Authenticated User Fakultas
Request :
- Method : GET
- Endpoint : `/api/user/{username}/fakultas`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "id" : "string",
         "nama_fakultas" : "string",
         "akreditasi" : "string"
    }
}
```
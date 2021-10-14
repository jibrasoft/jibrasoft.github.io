# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Homebase API Spec

## Authentication
No authentication needed to use this API

## Get Homebase
Request :
- Method : GET
- Endpoint : `/api/homebase/{idh}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
          "idh": "string",
          "nama": "string",
          "tgl_update": "datetime",
          "l": "integer",
          "p": "integer",
          "jlh": "integer"
    }
}
```

## List Homebase
Request :
- Method : GET
- Endpoint : `/api/homebase`
- Header :
    - Accept: application/json
Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
            "idh": "string",
            "nama": "string",
            "tgl_update": "datetime",
            "l": "integer",
            "p": "integer",
            "jlh": "integer"
        },
        {
            "idh": "string",
            "nama": "string",
            "tgl_update": "datetime",
            "l": "integer",
            "p": "integer",
            "jlh": "integer"
        }
    ]
}
```
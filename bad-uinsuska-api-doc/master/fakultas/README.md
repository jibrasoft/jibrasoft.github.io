# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Dosen API Spec

## Authentication
No authentication needed to use this API

## Get Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen/{nip}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "idh" : "string",
         "nip" : "string",
         "nma" : "string",
         "email" : "string",
         "homebase": {
             "nma": "string",
             "tgl_update": "datetime",
             "idh": "string",
             "l": "integer",
             "p": "integer",
             "jlh": "integer"
         }
    }
}
```

## List Dosen
Request :
- Method : GET
- Endpoint : `/api/dosen`
- Header :
    - Accept: application/json
- Query Param :
    - idh : string
Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
            "idh" : "string",
            "nip" : "string",
            "nma" : "string",
            "email" : "string",
            "homebase": {
                "nma": "string",
                "tgl_update": "datetime",
                "idh": "string",
                "l": "integer",
                "p": "integer",
                "jlh": "integer"
            }
        },
        {
            "idh" : "string",
            "nip" : "string",
            "nma" : "string",
            "email" : "string",
            "homebase": {
                "nma": "string",
                "tgl_update": "datetime",
                "idh": "string",
                "l": "integer",
                "p": "integer",
                "jlh": "integer"
            }
        }
    ]
}
```
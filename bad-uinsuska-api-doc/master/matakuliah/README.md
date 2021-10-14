# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Matakuliah API Spec

## Authentication
No authentication needed to use this API

## Get Matakuliah
Request :
- Method : GET
- Endpoint : `/api/matakuliah/{id}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "id" : "string,unique",
         "idh" : "string",
         "kode" : "string,unique",
         "nama" : "string",
         "sks" : "integer",
         "semester" : "string",
         "kurikulum" : "string",
         "homebase": {
             "idh": "string",
             "nama": "string",
             "tgl_update": "datetime",
             "l": "integer",
             "p": "integer",
             "jlh": "integer"
         }
    }
}
```

## List Matakuliah
Request :
- Method : GET
- Endpoint : `/api/matakuliah`
- Header :
    - Accept: application/json
- Query Param :
    - idh : string
    - kurikulum : string
    - semester : string
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "id" : "string,unique",
             "idh" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "kurikulum" : "string",
             "homebase": {
                 "idh": "string",
                 "nama": "string",
                 "tgl_update": "datetime",
                 "l": "integer",
                 "p": "integer",
                 "jlh": "integer"
             }
        },
        {
             "id" : "string,unique",
             "idh" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "kurikulum" : "string",
             "homebase": {
                 "idh": "string",
                 "nama": "string",
                 "tgl_update": "datetime",
                 "l": "integer",
                 "p": "integer",
                 "jlh": "integer"
             }
        }
    ]
}
```
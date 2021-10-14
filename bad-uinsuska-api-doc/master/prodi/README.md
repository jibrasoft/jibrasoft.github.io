# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Prodi API Spec

## Authentication
No authentication needed to use this API

## Get Prodi
Request :
- Method : GET
- Endpoint : `/api/prodi/{id}`
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
         "idf" : "string",
         "nama_prodi" : "string",
         "akreditasi" : "string",
         "fakultas" : {
             "id" : "string",
             "nama_fakultas" : "string",
             "akreditasi" : "string"
         }
    }
}
```

## List Prodi
Request :
- Method : GET
- Endpoint : `/api/prodi`
- Header :
    - Accept: application/json
- Query Param : 
    - idf : string
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "id" : "string",
             "idf" : "string",
             "nama_prodi" : "string",
             "akreditasi" : "string",
             "fakultas" : {
                 "id" : "string",
                 "nama_fakultas" : "string",
                 "akreditasi" : "string"
             }
        },
        {
            "id" : "string",
            "idf" : "string",
            "nama_prodi" : "string",
            "akreditasi" : "string",
            "fakultas" : {
                 "id" : "string",
                 "nama_fakultas" : "string",
                 "akreditasi" : "string"
            }
        }
    ]
}
```
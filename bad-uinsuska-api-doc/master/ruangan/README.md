# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Ruangan API Spec

## Authentication
No authentication needed to use this API

## Get Ruangan
Request :
- Method : GET
- Endpoint : `/api/ruangan/{id}`
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
         "kode_ruangan" : "string",
         "keterangan" : "string",
         "fakultas" : {
             "id" : "string",
             "nama_fakultas" : "string",
             "akreditasi" : "string"
         }
    }
}
```

## List Ruangan
Request :
- Method : GET
- Endpoint : `/api/ruangan`
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
             "kode_ruangan" : "string",
             "keterangan" : "string",
             "fakultas" : {
                 "id" : "string",
                 "nama_fakultas" : "string",
                 "akreditasi" : "string"
             }
        },
        {
            "id" : "string",
            "idf" : "string",
            "kode_ruangan" : "string",
            "keterangan" : "string",
            "fakultas" : {
                "id" : "string",
                "nama_fakultas" : "string",
                "akreditasi" : "string"
            }
        }
    ]
}
```
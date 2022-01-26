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
         "id" : "integer",
         "idp" : "string",
         "kode" : "string,unique",
         "nama" : "string",
         "sks" : "integer",
         "semester" : "string",
         "prodi" : {
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
}
```

## List Matakuliah
Request :
- Method : GET
- Endpoint : `/api/matakuliah`
- Header :
    - Accept: application/json
- Query Param :
    - idp : string
    - semester : string
    - page : integer
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "id" : "integer",
             "idp" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "prodi" : {
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
        },
        {
             "id" : "integer",
             "idp" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "prodi" : {
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
    ]
}
```

## Get Authenticated User Matakuliah
Request :
- Method : GET
- Endpoint : `/api/user/{username}/matakuliah`
- Header :
    - Accept: application/json
- Query Param :
    - idp : string
    - semester : string
    - page : integer
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "id" : "integer",
             "idp" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "prodi" : {
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
        },
        {
             "id" : "integer",
             "idp" : "string",
             "kode" : "string,unique",
             "nama" : "string",
             "sks" : "integer",
             "semester" : "string",
             "prodi" : {
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
    ]
}
```
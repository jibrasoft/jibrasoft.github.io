# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Dosen LB API Spec

## Authentication
No authentication needed to use this API

## Get Dosen LB
Request :
- Method : GET
- Endpoint : `/api/dosen/lb/{nip}`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "nip" : "string",
         "idp" : "string",
         "idj" : "string|null",
         "nama" : "string",
         "nidn_nup" : "string",
         "golongan_jabatan" : "string",
         "email" : "string",
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

## List Dosen LB
Request :
- Method : GET
- Endpoint : `/api/dosen/lb`
- Header :
    - Accept: application/json
- Query Param :
    - idp : string
    - nama : string
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "nip" : "string",
             "idp" : "string",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
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
             "nip" : "string",
             "idp" : "string",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
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

## List Authenticated User Dosen LB
Request :
- Method : GET
- Endpoint : `/api/user/{username}/dosen/lb`
- Header :
    - Accept: application/json
- Query Param :
    - nama : string
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : [
        {
             "nip" : "string",
             "idp" : "string",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
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
             "nip" : "string",
             "idp" : "string",
             "nama" : "string",
             "nidn_nup" : "string",
             "golongan_jabatan" : "string",
             "email" : "string",
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
# Sistem Informasi Beban Akademik Dosen Terintegrasi API Spec v1.0.0 

## Description
Semester API Spec

## Authentication
No authentication needed to use this API

## Get Active Semester
Request :
- Method : GET
- Endpoint : `/api/semester/aktif`
- Header :
    - Accept: application/json
- Response :

```json 
{
    "code" : "integer",
    "status" : "string",
    "message" : "string",
    "data" : {
         "id": "string",
         "nama_semester": "string",
         "a_periode_aktif": "enum[0,1]",
         "tgl_mulai": "date",
         "tgl_selesai": "date"
    }
}
```

## List Semester
Request :
- Method : GET
- Endpoint : `/api/semester`
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
            "id": "string",
            "nama_semester": "string",
            "a_periode_aktif": "enum[0,1]",
            "tgl_mulai": "date",
            "tgl_selesai": "date"
        },
        {
            "id": "string",
            "nama_semester": "string",
            "a_periode_aktif": "enum[0,1]",
            "tgl_mulai": "date",
            "tgl_selesai": "date"
        }
    ]
}
```
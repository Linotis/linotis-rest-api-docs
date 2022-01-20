# Language list
Return all language list.

```
GET http/{{host}}/languages
```
## Parameters
### Header parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| Authorization  | Y| String |
### URI Parameters

None

### Body Parameters

None

## Response
### Success Response
```
Code: 200
Content: [
    {
        "collections": [],
        "_id": "61df0f8e9fccc52efc68b687",
        "name": "de",
        "icon": "",
        "__v": 0
    },
    {
        "_id": "61df153def90c7ab49447cfd",
        "name": "en",
        "icon": "",
        "collections": [
            "61df17f3887bb6a12260461e"
        ],
        "__v": 1
    },
    {
        "_id": "61e98e2a271b8f4b7c71d9fe",
        "name": "fr",
        "icon": "",
        "collections": [],
        "__v": 0
    }
]
```
### Error Response
```
Code: 401
Content: Unauthorized
```

## Sample call
```
curl --location --request GET 'http://localhost:5000/api/languages/' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzI4LmNvbSIsInVzZXJJZCI6IjYxZDM3ZTNjYmFiYjFiODRiZGJjNzUwMCIsImlhdCI6MTY0MjY5NDAyMCwiZXhwIjoxNjQyNjk3NjIwfQ.wmgWfdIG5ipc5KJDXun_ncYQU1vmP-alq4b0XEOkgEQ' \
--data-raw ''
```
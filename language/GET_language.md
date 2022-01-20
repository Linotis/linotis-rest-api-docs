# Language
Return language by id.

```
GET http/{{host}}/language/:id
```
## Parameters
### URI Parameters

| Field  | Required | Type|
| ------------- | ------------- | ----- |
| id  | Y| String |
### Header parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| Authorization  | Y| String |

### Body Parameters

None

## Response
### Success Response
```
Code: 200
Content: {
    "_id": "61df153def90c7ab49447cfd",
    "name": "en",
    "icon": "",
    "collections": [
        {
            "_id": "61df17f3887bb6a12260461e",
            "name": "testNewCollection",
            "scribbles": [],
            "languageId": "61df153def90c7ab49447cfd",
            "__v": 0
        }
    ],
    "__v": 1
}
```
### Error Response
```
Code: 401
Content: Unauthorized
```
OR
```
Code: 400
Content: Language not found
```

## Sample call
```
curl --location --request GET 'http://localhost:5000/api/language/61df153def90c7ab49447cfd' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzI4LmNvbSIsInVzZXJJZCI6IjYxZDM3ZTNjYmFiYjFiODRiZGJjNzUwMCIsImlhdCI6MTY0MjY5NDAyMCwiZXhwIjoxNjQyNjk3NjIwfQ.wmgWfdIG5ipc5KJDXun_ncYQU1vmP-alq4b0XEOkgEQ' \
--data-raw ''
```
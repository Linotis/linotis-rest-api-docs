# Add language
Create new language.

```
POST http/{{host}}/language
```
## Parameters

### URI Parameters

None
### Header parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| Authorization  | Y| String |
### Body Parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| name  | Y| String |
| icon  | Y| String |

## Response
### Success Response
```
Code: 201
{
    "name": "fr",
    "icon": "",
    "collections": [],
    "_id": "61e98e2a271b8f4b7c71d9fe",
    "__v": 0
}
```
### Error Response
```
Code: 401
Content: Unauthorized
```
OR
```
Code: 500
Content: Collection validation failed: name: Path `name` is required.
```

## Sample call
```
curl --location --request POST 'http://localhost:5000/api/language' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzI4LmNvbSIsInVzZXJJZCI6IjYxZDM3ZTNjYmFiYjFiODRiZGJjNzUwMCIsImlhdCI6MTY0MjY5NDAyMCwiZXhwIjoxNjQyNjk3NjIwfQ.wmgWfdIG5ipc5KJDXun_ncYQU1vmP-alq4b0XEOkgEQ' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "fr" 
}'
```
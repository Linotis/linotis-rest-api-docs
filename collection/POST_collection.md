# Create collection
Create new collection.

```
POST http/{{host}}/collection
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

## Response
### Success Response
```
Code: 201
Content: {
    "name": "testNewCollection",
    "scribbles": [],
    "_id": "61c73ea12911815bbf49d264",
    "__v": 0
}
```
### Error Response
```
Code: 401
Content: Unauthorized
```

## Sample call
```
curl --location --request POST 'http://localhost:5000/api/collection' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzIuY29tIiwidXNlcklkIjoiNjFiNWEyZDc3ZGI1MzI1ZTE3NWM3OGY2IiwiaWF0IjoxNjQwNDQ3MjQ0LCJleHAiOjE2NDA0NTA4NDR9.Tna84LLvyH8BB3tKVnUKAmuNQ4bSmNalJjyYATvLIX8' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "testNewCollection"
}'
```
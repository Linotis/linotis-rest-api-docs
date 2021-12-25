# Collection
Return collection by id.

```
GET http/{{host}}/collection/:id
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
    "_id": "61b8da553d2252b08bd355d8",
    "name": "testNewCollection",
    "scribbles": [],
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
Code: 400
Content: Collection not found
```

## Sample call
```
curl --location --request GET 'http://localhost:5000/api/collection/61c73edc2911815bbf49d267' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzIuY29tIiwidXNlcklkIjoiNjFiNWEyZDc3ZGI1MzI1ZTE3NWM3OGY2IiwiaWF0IjoxNjQwNDQ3MjQ0LCJleHAiOjE2NDA0NTA4NDR9.Tna84LLvyH8BB3tKVnUKAmuNQ4bSmNalJjyYATvLIX8'
```
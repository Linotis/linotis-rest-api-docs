# Update collection
Update collection name.

```
PATCH http/{{host}}/collection/:id
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
    "_id": "61c73edc2911815bbf49d267",
    "scribbles": [],
    "__v": 0,
    "name": "testUpdateCollectionName"
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
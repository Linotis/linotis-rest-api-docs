# Delete collection
Delete collection by id.

```
DELETE http/{{host}}/collection/:id
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
Content: Collection delete
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
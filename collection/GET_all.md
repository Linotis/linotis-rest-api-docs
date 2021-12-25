# Collections list
Return all collection list.

```
GET http/{{host}}/collections
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
        "_id": "61b8da553d2252b08bd355d8",
        "name": "testNewCollection",
        "scribbles": [],
        "__v": 0
    },
    {
        "_id": "61b8da903d2252b08bd355db",
        "name": "testNewCollection",
        "scribbles": [],
        "__v": 0
    },
    {
        "_id": "61bf7b744055868f840dd64e",
        "name": "testNewCollection",
        "scribbles": [
            "61bf7c89ff057bf0949b4d6f",
            "61c4c73e69504dd9a9e351bf",
            "61c4c7c669504dd9a9e351c4",
            "61c4cb3369504dd9a9e351cb",
            "61c4cb7069504dd9a9e351d0"
        ],
        "__v": 5
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
curl --location --request GET 'http://localhost:5000/api/collections' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtbzIuY29tIiwidXNlcklkIjoiNjFiNWEyZDc3ZGI1MzI1ZTE3NWM3OGY2IiwiaWF0IjoxNjQwNDQ3MjQ0LCJleHAiOjE2NDA0NTA4NDR9.Tna84LLvyH8BB3tKVnUKAmuNQ4bSmNalJjyYATvLIX8'
```
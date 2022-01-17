# Upadte User info
Update user information.

```
PATCH http/{{host}}/api/user
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
| email  | N| String |
| firstName  | N| String |
| lastName  | N| String |
| agr | N| String |
| role | N| String |
| languages  | N| String |

## Response
### Success Response
```
Code: 201
Content: {
    "_id": "61d74b9530913065245b8c16",
    "email": "demo@demo.com",
    "password": "$2a$10$dKjbBDT5ppzuSBVTCMtpHe01T.u19bJ27JyPil0P0gypNekdQ0QzO",
    "firstName": "newUser",
    "lastName": "demo",
    "age": 30,
    "role": "student",
    "__v": 0,
    "languages": [
        "61df0f8e9fccc52efc68b687"
    ]
}
```
### Error Response
```
Code: 401
Content: Unauthorized
```

## Sample call
```
curl --location --request PATCH 'http://localhost:5000/api/user' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtby5jb20iLCJ1c2VySWQiOiI2MWQ3NGI5NTMwOTEzMDY1MjQ1YjhjMTYiLCJpYXQiOjE2NDI0NDM1MTcsImV4cCI6MTY0MjQ0NzExN30.xoZicmJCZQQZNUaI_rYtU6OX4Q3bhKa1uaTCvsHKMCg' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName": "newUser",
    "age": 30,
    "languages": [
        {
            "_id": "61df0f8e9fccc52efc68b687",
            "name": "de"
        }
    ]
}'
```
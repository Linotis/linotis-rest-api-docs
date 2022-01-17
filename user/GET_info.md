# Get User info
Getting user information.

```
GET http/{{host}}/api/user
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
        {
            "collections": [],
            "_id": "61df0f8e9fccc52efc68b687",
            "name": "de",
            "icon": "",
            "__v": 0
        }
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
curl --location --request GET 'http://localhost:5000/api/user' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImRlbW9AZGVtby5jb20iLCJ1c2VySWQiOiI2MWQ3NGI5NTMwOTEzMDY1MjQ1YjhjMTYiLCJpYXQiOjE2NDI0NDM1MTcsImV4cCI6MTY0MjQ0NzExN30.xoZicmJCZQQZNUaI_rYtU6OX4Q3bhKa1uaTCvsHKMCg'
```
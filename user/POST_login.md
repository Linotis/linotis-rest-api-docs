# Register User
Makes a login for the user.

```
POST http/{{host}}/auth/login
```
## Parameters
### URI Parameters

None

### Body Parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| email  | Y| String |
| password  | Y| String |

## Response
### Success Response
```
Code: 200
Content: { token: "token": "Bearer token"}
```
### Error Response
```
Code: 400
Content: { message: "Invalid password"}
```
OR
```
Code: 400
Content: { message: "User not found"}
```

## Sample call
```
curl --location --request POST 'http://localhost:5000/api/auth/login' \
--header 'Content-Type: application/json' \
--data-raw '{
    "email": "demo@demo2.com",
    "password": "demodemo2"
}'
```
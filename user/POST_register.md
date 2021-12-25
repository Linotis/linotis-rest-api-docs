# Register User
Makes the registration of a new user.

```
POST http/{{host}}/auth/register
```
## Parameters
### URI Parameters

None

### Body Parameters
| Field  | Required | Type|
| ------------- | ------------- | ----- |
| email  | Y| String |
| password  | Y| String |
| firstName  | Y| String |
| lastName  | Y| String |
| age  | Y| Number |
| role  | Y| String |

## Response
### Success Response
```
Code: 200
Content: { message: "Ok"}
```
### Error Response
```
Code: 400
Content: { message: "User demo@demo11.com already exists"}
```

## Sample call
```
curl --location --request POST 'http://localhost:5000/api/auth/register' \
--header 'Content-Type: application/json' \
--data-raw '{
    "email": "demo@demo11.com",
    "password": "demodemo11",
    "firstName": "A",
    "lastName": "B",
    "age": 20,
    "role": "student"
}'
```

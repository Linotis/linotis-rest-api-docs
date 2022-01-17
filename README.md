# Linotis REST API
## Overview
Linotis is a service for learning foreign languages by writing words and letters. Linotis API contains a description of the methods used in the service.
## API Versioning
No version available at this time
## HTTP requests
All API requests are performed by sending an HTTP request using one of the following methods, depending on the action being performed:
- `POST` Create a resource
- `PATCH` Update a resource
- `GET` Get a resource or list of resources
- `DELETE` Delete a resource
## HTTP Response Codes
Each response will be returned with one of the following HTTP status codes:
- `200` `OK` The request was successful
- `201` `Created` New resource being created or updated
- `400` `Bad request` There was a problem with the request
- `401` `Unauthorized` The supplied API credentials are invalid
- `500` `Server Error` An error on the server occurred
## Resource list
### User
- [**`POST` Register user**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/user/POST_register.md)
- [**`POST` Login user**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/user/POST_login.md)
- [**`GET` User info**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/user/GET_info.md)
- [**`PATCH` Update user info**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/user/PATCH_info.md)
### Collection
- [**`POST` Create collection**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/POST_collection.md)
- [**`GET` All collections list**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_all.md)
- [**`GET` Collection**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_collection.md)
- [**`PATCH` Update collection**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/PATCH_collection.md)
- [**`DELETE` Delete collection**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/DELETE_collection.md)

### Scribble
- [**`POST` Create scribble**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/POST_collection.md)
- [**`GET` All scribble list**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_all.md)
- [**`GET` Scribble**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_collection.md)
- [**`PATCH` Update scribble**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/PATCH_collection.md)
- [**`DELETE` Delete scribble**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/DELETE_collection.md)
### Language
- [**`POST` Add language**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/POST_collection.md)
- [**`GET` All languages list**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_all.md)
- [**`GET` Language**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/GET_collection.md)
- [**`PATCH` Update language**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/PATCH_collection.md)
- [**`DELETE` Delete language**](https://github.com/Linotis/linotis-rest-api-docs/blob/main/collection/DELETE_collection.md)

## License
Copyright (C)  2021  Linotis.

Permission is granted to copy, distribute and/or modify this document
under the terms of the GNU Free Documentation License, Version 1.3
or any later version published by the Free Software Foundation;
with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
A copy of the license is included in the section entitled "GNU
Free Documentation License".

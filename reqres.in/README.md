# Postman

URL: https://reqres.in/
***

*1. Show list of users*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/List%20Users%20-%20Valid.png)
</details>

```
Method: GET
EndPoint: api/users
Request url params: 
	page: 1

Response: 
{
    "page": 1,
    "per_page": 6,
    "total": 12,
    "total_pages": 2,
    "data": [
        {
            "id": 1,
            "email": "george.bluth@reqres.in",
            "first_name": "George",
            "last_name": "Bluth",
            "avatar": "https://reqres.in/img/faces/1-image.jpg"
        },
        {
            "id": 2,
            "email": "janet.weaver@reqres.in",
            "first_name": "Janet",
            "last_name": "Weaver",
            "avatar": "https://reqres.in/img/faces/2-image.jpg"
        },
        {
            "id": 3,
            "email": "emma.wong@reqres.in",
            "first_name": "Emma",
            "last_name": "Wong",
            "avatar": "https://reqres.in/img/faces/3-image.jpg"
        },
        {
            "id": 4,
            "email": "eve.holt@reqres.in",
            "first_name": "Eve",
            "last_name": "Holt",
            "avatar": "https://reqres.in/img/faces/4-image.jpg"
        },
        {
            "id": 5,
            "email": "charles.morris@reqres.in",
            "first_name": "Charles",
            "last_name": "Morris",
            "avatar": "https://reqres.in/img/faces/5-image.jpg"
        },
        {
            "id": 6,
            "email": "tracey.ramos@reqres.in",
            "first_name": "Tracey",
            "last_name": "Ramos",
            "avatar": "https://reqres.in/img/faces/6-image.jpg"
        }
    ],
    "support": {
        "url": "https://reqres.in/#support-heading",
        "text": "To keep ReqRes free, contributions towards server costs are appreciated!"
    }
}
```

*2. Show single user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Single%20User%20-%20Valid.png)
</details>

```
Method: GET
EndPoint: /api/users/2

Response: 
{
    "data": {
        "id": 2,
        "email": "janet.weaver@reqres.in",
        "first_name": "Janet",
        "last_name": "Weaver",
        "avatar": "https://reqres.in/img/faces/2-image.jpg"
    },
    "support": {
        "url": "https://reqres.in/#support-heading",
        "text": "To keep ReqRes free, contributions towards server costs are appreciated!"
    }
}
```

*3. Show list RESOURCE*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/list%20Resource%20-%20valid.png)
</details>

```
Method: GET
EndPoint: /api/unknown

Response:
{
    "page": 1,
    "per_page": 6,
    "total": 12,
    "total_pages": 2,
    "data": [
        {
            "id": 1,
            "name": "cerulean",
            "year": 2000,
            "color": "#98B2D1",
            "pantone_value": "15-4020"
        },
        {
            "id": 2,
            "name": "fuchsia rose",
            "year": 2001,
            "color": "#C74375",
            "pantone_value": "17-2031"
        },
        {
            "id": 3,
            "name": "true red",
            "year": 2002,
            "color": "#BF1932",
            "pantone_value": "19-1664"
        },
        {
            "id": 4,
            "name": "aqua sky",
            "year": 2003,
            "color": "#7BC4C4",
            "pantone_value": "14-4811"
        },
        {
            "id": 5,
            "name": "tigerlily",
            "year": 2004,
            "color": "#E2583E",
            "pantone_value": "17-1456"
        },
        {
            "id": 6,
            "name": "blue turquoise",
            "year": 2005,
            "color": "#53B0AE",
            "pantone_value": "15-5217"
        }
    ],
    "support": {
        "url": "https://reqres.in/#support-heading",
        "text": "To keep ReqRes free, contributions towards server costs are appreciated!"
    }
}

```
*4. Show single RESOURCE*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Single%20Resource%20-%20Valid.png)
</details>

```
Method: GET
EndPoint: /api/unknown/4

Response:
{
    "data": {
        "id": 4,
        "name": "aqua sky",
        "year": 2003,
        "color": "#7BC4C4",
        "pantone_value": "14-4811"
    },
    "support": {
        "url": "https://reqres.in/#support-heading",
        "text": "To keep ReqRes free, contributions towards server costs are appreciated!"
    }
}
```

*5. Delayed response*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Delayed%20Response.png)
</details>

```
Method: GET
EndPoint: /api/users
Request url params: 
	delay: 5

Response:
Time - 5.12 s
{
    "page": 1,
    "per_page": 6,
    "total": 12,
    "total_pages": 2,
    "data": [
        {
            "id": 1,
            "email": "george.bluth@reqres.in",
            "first_name": "George",
            "last_name": "Bluth",
            "avatar": "https://reqres.in/img/faces/1-image.jpg"
        },
        {
            "id": 2,
            "email": "janet.weaver@reqres.in",
            "first_name": "Janet",
            "last_name": "Weaver",
            "avatar": "https://reqres.in/img/faces/2-image.jpg"
        },
        {
            "id": 3,
            "email": "emma.wong@reqres.in",
            "first_name": "Emma",
            "last_name": "Wong",
            "avatar": "https://reqres.in/img/faces/3-image.jpg"
        },
        {
            "id": 4,
            "email": "eve.holt@reqres.in",
            "first_name": "Eve",
            "last_name": "Holt",
            "avatar": "https://reqres.in/img/faces/4-image.jpg"
        },
        {
            "id": 5,
            "email": "charles.morris@reqres.in",
            "first_name": "Charles",
            "last_name": "Morris",
            "avatar": "https://reqres.in/img/faces/5-image.jpg"
        },
        {
            "id": 6,
            "email": "tracey.ramos@reqres.in",
            "first_name": "Tracey",
            "last_name": "Ramos",
            "avatar": "https://reqres.in/img/faces/6-image.jpg"
        }
    ],
    "support": {
        "url": "https://reqres.in/#support-heading",
        "text": "To keep ReqRes free, contributions towards server costs are appreciated!"
    }
}
```

*6. Show single user - invalid*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Single%20User%20-%20Invalid.png)
</details>

```
Method: GET
EndPoint: /api/users/23

Response:
{}
```

*7. Show single RESOURCE*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Single%20Resource%20-%20Invalid.png)
</details>

```
Method: GET
EndPoint: /api/unknown/23

Response:
{}
```
*8. Create a user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Create%20User%20-%20Valid.png)
</details>

```
Method: POST
EndPoint: /api/users
Body:
{
    "name": "morpheus",
    "job": "leader"
}

Response:
{
    "name": "morpheus",
    "job": "leader",
    "id": "806",
    "createdAt": "2022-12-23T17:45:56.469Z"
}
```

*9. Register a user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Register%20-%20Valid.png)
</details>

```
Method: POST
EndPoint: /api/register
Body:
{
    "email": "eve.holt@reqres.in",
    "password": "pistol"
}

Response:
{
    "id": 4,
    "token": "QpwL5tke4Pnpja7X4"
}
```

*10. Login*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Login%20-%20Valid.png)
</details>

```
Method: POST
EndPoint: /api/login
Body:
{
    "email": "eve.holt@reqres.in",
    "password": "cityslicka"
}

Response:
{
    "token": "QpwL5tke4Pnpja7X4"
}
```

*11. Register a user - invalid*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Register%20-%20Invalid.png)
</details>

```
Method: POST
EndPoint: /api/register
Body:
{
    "email": "sydney@fife"
}

Response:
{
    "error": "Missing password"
}
```

*12. Login - invalid*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Login%20-%20Invalid.png)
</details>

```
Method: POST
EndPoint: /api/login
Body:
{
    "email": "peter@klaven"
}

Response:
{
    "error": "Missing password"
}
```

*13. Update a user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Update.png)
</details>

```
Method: PUT
EndPoint: api/users/2
Body:
{
    "name": "morpheus",
    "job": "zion resident"
}

Response:
{
    "name": "morpheus",
    "job": "zion resident",
    "updatedAt": "2022-12-23T18:01:18.039Z"
}
```

*14. Update a user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Update%20(PATCH).png)
</details>

```
Method: PATCH
EndPoint: /api/users/2
Body:
{
    "name": "morpheus",
    "job": "zion resident"
}

Response:
{
    "name": "morpheus",
    "job": "zion resident",
    "updatedAt": "2022-12-23T18:04:24.443Z"
}
```

*15. Delete a user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/reqres.in/Screens/Delete.png)
</details>

```
Method: DELETE
EndPoint: /api/users/2
Response: Stutus: 204 No Content
```


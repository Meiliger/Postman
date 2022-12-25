# Postman

Base URL: petstore.swagger.io/v2
***

## User

*1. Create user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/1.png)
</details>

```
Method: POST
EndPoint: /user
Body:
{
  "id": 4,
  "username": "andrey34324",
  "firstName": "Andrey",
  "lastName": "Vakulovich",
  "email": "test@mail.com",
  "password": "1234",
  "phone": "+380999999999",
  "userStatus": 1
}

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "4"
}
```
***

*2. Get user by username*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/2.png)
</details>

```
Method: GET
EndPoint: /user/{{username}}
Response:
{
    "id": 4,
    "username": "andrey34324",
    "firstName": "Andrey",
    "lastName": "Vakulovich",
    "email": "test@mail.com",
    "password": "1234",
    "phone": "+380999999999",
    "userStatus": 1
}
```
***

*3. Logs user in the system*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/3.png)
</details>

```
Method: GET
EndPoint: /user/login
Request url params: 
	username: andrey34324
	password: 1234

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "logged in user session:1671980344834"
}
```
***

*4. Logs user out the system*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/4.png)
</details>

```
Method: GET
EndPoint: /user/logout

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "ok"
}
```
***

*5. Update user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](5)
</details>

```
Method: PUT
EndPoint: /user/{{username}}

Body:
{
    "id": 4,
    "username": "andrey34324",
    "firstName": "Andrey",
    "lastName": "Vakulovich",
    "email": "newtest@mail.com",
    "password": "5678",
    "phone": "+380777777777",
    "userStatus": 1
}

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "4"
}
```

<details>
  <summary>Get user by username</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/5(3).png)
</details>

***

*6. Creates list of users with given input array*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/6.png)
</details>

```
Method: POST
EndPoint: /user/createWithArray

Body:
[
  {
    "id": 2,
    "username": "newuser",
    "firstName": "user1",
    "lastName": "testname1",
    "email": "newuser1@mail.com",
    "password": "qwerty",
    "phone": "+380955555555",
    "userStatus": 5
  },
    {
    "id": 2,
    "username": "newuser22",
    "firstName": "user2",
    "lastName": "testname2",
    "email": "newuser2222@mail.com",
    "password": "dsdf32341",
    "phone": "+380987654321",
    "userStatus": 6
  },
      {
    "id": 2,
    "username": "newuser3333",
    "firstName": "user3",
    "lastName": "testname3",
    "email": "newuser2222@mail.com",
    "password": "dsdf32341",
    "phone": "+380987654321",
    "userStatus": 6
  }
]

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "ok"
}
```
***

*7. Delete user*

<details>
  <summary>Screenshot</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/7.png)
</details>

```
Method: DELETE
EndPoint: /user/{{username}}

Response:
{
    "code": 200,
    "type": "unknown",
    "message": "andrey34324"
}
```

<details>
  <summary>Get user by username</summary>
  
  ![Postman](https://github.com/Meiliger/postman/blob/main/petstore/Screens/user/8.png)
</details>



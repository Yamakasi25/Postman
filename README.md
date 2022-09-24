# Postman
post request (registration) https://blog.kata.academy/api/users

body: { 
   "user": {
    "username": "test2",
    "email": "test@mail.ru",
    "password": "12345qwerty"
  }}
  
  response: { "user": {
        "username": "test2",
        "email": "test@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMmVlZjkzM2NmNzA1MWIwMDgyYTgxMSIsInVzZXJuYW1lIjoidGVzdDIiLCJleHAiOjE2NjkyMDQzNzEsImlhdCI6MTY2NDAyMDM3MX0.dA3yKLljKx91v1yNzfFgaJsbCLuVrKOXFpI3jXu2tsw"
    }}
***    
post request (Authentication) https://blog.kata.academy/api/users/login

body: {
  "user": {
    "email": "test@mail.ru",
    "password": "12345qwerty"
  }
}

response: {
    "user": {
        "username": "test2",
        "email": "test@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMmVlZjkzM2NmNzA1MWIwMDgyYTgxMSIsInVzZXJuYW1lIjoidGVzdDIiLCJleHAiOjE2NjkyMDUyMDEsImlhdCI6MTY2NDAyMTIwMX0.-7v28M0tqHrmkIFAKpdXjpk4MRK5MOFkisbnlsdzK90"
    }
}
***
get request (Endpoint) https://blog.kata.academy/api/user

body {
  "user": {
    "username": "test2",
    "email": "test@mail.ru",
    "password": "12345qwerty"
  }
}

В Headers добавил Autorisation Token

Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMmVlZjkzM2NmNzA1MWIwMDgyYTgxMSIsInVzZXJuYW1lIjoidGVzdDIiLCJleHAiOjE2NjkyMDUyMDEsImlhdCI6MTY2NDAyMTIwMX0.-7v28M0tqHrmkIFAKpdXjpk4MRK5MOFkisbnlsdzK90

response: {
    "user": {
        "username": "test2",
        "email": "test@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMmVlZjkzM2NmNzA1MWIwMDgyYTgxMSIsInVzZXJuYW1lIjoidGVzdDIiLCJleHAiOjE2NjkyMDUyNDksImlhdCI6MTY2NDAyMTI0OX0.PsdCXY7oOp_4vkXBqkZ7SojXgxxaI7hXFk1vFm9B8_w"
    }
}

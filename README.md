# register-login-jwt

`POST` `/register`

**Sample Request Body:**

```json
{
  "first_name": "Ayush",
  "last_name": "Shaw",
  "email": "ayush@gmail.com",
  "password": "1234567890"
}
```

**Sample Response Body:**

```json
{
  "first_name": "Ayush",
  "last_name": "Shaw",
  "email": "ayush@gmail.com",
  "password": "$2a$10$ERCbbtX97yv95pH9FcKqAeiLGeyJ7LOJvdSjG8u2HYleqAhT6ekYG",
  "_id": "61653c9e09a1535274e66e71",
  "__v": 0,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjE2NTNjOWUwOWExNTM1Mjc0ZTY2ZTcxIiwiZW1haWwiOiJhcnBhbmFAZ21haWwuY29tIiwiaWF0IjoxNjM0MDI0NjA3LCJleHAiOjE2MzQwMzE4MDd9.3oJNjrfRxS2yKtx0uImsQ0-ndHSx55y4BbmSIC2JAIg"
}
```

---

`POST` `/login`

**Sample Request Body:**

```json
{
  "email": "ayushshawx@gmail.com",
  "password": "1234567890"
}
```

**Sample Response Body:**

```json
{
  "_id": "61652d9bed6b6136eb6b4e56",
  "first_name": "Ayush",
  "last_name": "Shaw",
  "email": "ayushshawx@gmail.com",
  "password": "$2a$10$ZvIbxTaERW1I6saHD6gIu.HBKYJoc/f8w1EEO1eSb0rJjbAMK1hCK",
  "__v": 0,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjE2NTJkOWJlZDZiNjEzNmViNmI0ZTU2IiwiZW1haWwiOiJheXVzaHNoYXd4QGdtYWlsLmNvbSIsImlhdCI6MTYzNDAyNDg0NSwiZXhwIjoxNjM0MDMyMDQ1fQ.sSlv_JcmpLhlsLOQs2QuxL6I1WO2tEiqRiVFuMG0thM"
}
```

---

`POST` `/welcome`

**Sample Request Body:**

```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjE2NTJkOWJlZDZiNjEzNmViNmI0ZTU2IiwiZW1haWwiOiJheXVzaHNoYXd4QGdtYWlsLmNvbSIsImlhdCI6MTYzNDAyMDkwNCwiZXhwIjoxNjM0MDI4MTA0fQ.Iw-BTjAcl3SK2v-uylLCCuzUu7_Cqw62Gh0I2mlrLDA"
}
```

**Sample Response Body:**

```json
Welcome 🙌 Ayush 👋
```

[**NOTE:** The `/welcome` endpoint also supports `token` as a query param and `x-access-token` as a header.]

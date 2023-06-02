---
sidebar_position: 4
---

# Register User

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can register.

## 3. API

### Register User Request example:

```json
{
  "UserName": "username",
  "Email": "user@example.com",
  "Password": "123456",
  "CreatedAt": "2020-03-24T06:03:00.348+03:00"
}
```

### Create User Response example:

```json
{
   "Data":{
      "User":{
         "ID":"123e4567-e89b-12d3-a456-426614174000"
      }
   }
}
`
```

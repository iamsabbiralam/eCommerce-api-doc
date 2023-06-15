---
sidebar_position: 2
---

# Seller Registration

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-commerce seller can register.

## 3. API

### Create Seller Request example:

```json
{
  "Email": "seller@example.com",
  "Password": "12345678",
  "Status": "PENDING",
  "CreatedAt": "2020-03-24T06:03:00.348+03:00"
}
```

### Create Seller Response example:

```json
{
   "Data":{
      "Seller":{
         "ID":"123e4567-e89b-12d3-a456-426614174000"
      }
   }
}
```

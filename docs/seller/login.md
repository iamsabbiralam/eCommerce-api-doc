---
sidebar_position: 3
---

# Login

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce Seller can login to their profile.

## 3. API

### List Seller Request example:

```json
{
  "Email": "seller@example.com",
  "Password": "12345678"
}
```

### List Seller Response example:

```json
{
  "Data": {
    "Seller": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000"
      }
    ]
  }
}
```

---
sidebar_position: 5
---

# Login

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can login to their profile.

## 3. API

### List user Request example:

```json
{
  "Email": "user@example.com",
  "Password": "123456"
}
```

### List user Response example:

```json
{
  "Data": {
    "User": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000"
      }
    ]
  }
}
```

---
sidebar_position: 4
---

# Get Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-commerce admin can get details by ID or Name.

## 3. API

### Get Category Request example:

```json
{
  "Name": "Cloth"
}
```

### Get Category Response example:

```json
{
  "Data": {
    "Category": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Name": "Cloth",
      "IsActive": "1",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

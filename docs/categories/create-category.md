---
sidebar_position: 3
---

# Create Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can add new category.

## 3. API

### Create Category Request example:

```json
{
  "Name": "Cloth",
  "IsActive": "1",
  "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Create Category Response example:

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

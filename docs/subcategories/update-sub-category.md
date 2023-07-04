---
sidebar_position: 10
---

# Update Sub Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can Update sub category.

## 3. API

### Update Sub Category Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
  "Name": "Geans",
  "IsActive": "1"
}
```

### Get Sub Category Response example:

```json
{
  "Data": {
    "SubCategory": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
      "Name": "Geans",
      "IsActive": "1",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

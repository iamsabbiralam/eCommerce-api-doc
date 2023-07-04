---
sidebar_position: 6
---

# List Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can get category list.

## 3. API

### List Category Request example:

```json
{
  "SortBy": "DESC",
  "OrderByData": "name",
  "SearchTerm": "B",
  "Limit": "10",
  "Offset": "0",
  "IsActive": ""
}
```

### List Category Response example:

```json
{
  "Data": {
    "Currency": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Cloth",
        "IsActive": "1",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Electronics",
        "IsActive": "1",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
      }
    ],
    "Total": 2
  }
}
```

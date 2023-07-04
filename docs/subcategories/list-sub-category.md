---
sidebar_position: 11
---

# List Sub Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can get sub category list.

## 3. API

### List Sub Category Request example:

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

### List Sub Category Response example:

```json
{
  "Data": {
    "Currency": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
        "Name": "T-Shirt",
        "IsActive": "1",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
        "Name": "Geans",
        "IsActive": "1",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
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

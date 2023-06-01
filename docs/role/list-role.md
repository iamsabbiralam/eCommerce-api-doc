---
sidebar_position: 7
---

# List Role

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can get role list.

## 3. API

### List Role Request example:

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

### List Role Response example:

```json
{
  "Data": {
    "Role": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Super-Admin",
        "Description": "This is super admin update",
        "IsActive": "INACTIVE",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Admin",
        "Description": "This is admin update",
        "IsActive": "ACTIVE",
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

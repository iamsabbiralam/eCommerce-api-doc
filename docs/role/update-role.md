---
sidebar_position: 6
---

# Update Role

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can Update role.

## 3. API

### Update Role Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "Name": "Super-Admin",
  "Description": "This is super admin update",
  "IsActive": "INACTIVE"
}
```

### Get Role Response example:

```json
{
  "Data": {
    "Role": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Name": "Super-Admin",
      "Description": "This is super admin update",
      "IsActive": "INACTIVE",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

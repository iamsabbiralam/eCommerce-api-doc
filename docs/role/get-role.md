---
sidebar_position: 5
---

# Get Role

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can get details by ID of role.

## 3. API

### Get Role Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get Role Response example:

```json
{
  "Data": {
    "Role": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Name": "SuperAdmin",
      "Description": "This is super admin",
      "IsActive": "ACTIVE",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

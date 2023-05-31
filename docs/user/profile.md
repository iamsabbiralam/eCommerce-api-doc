---
sidebar_position: 5
---

# Profile

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can get details by ID.

## 3. API

### Profile Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Profile Response example:

```json
{
  "Data": {
    "User": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Avatar": "",
      "FirstName": "",
      "LastName": "",
      "UserName": "username",
      "Email": "user@example.com",
      "Phone": "",
      "Gender": "",
      "Dob": "",
      "PermanentAddress": "",
      "City": "",
      "Country": "",
      "IsActive": "ACTIVE",
      "IsSuperAdmin": "INACTIVE",
      "IsEmailVerified": "ACTIVE",
      "MFAType": "EMAIL",
      "IsMfa": "ACTIVE",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "",
      "UpdatedAt": "",
      "UpdatedBy": ""
    }
  }
}
```

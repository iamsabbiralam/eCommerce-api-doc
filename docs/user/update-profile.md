---
sidebar_position: 7
---

# Update profile

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can Update their profile.

## 3. API

### Update profile Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "Avatar": "avatar.jpg",
  "FirstName": "first",
  "LastName": "last",
  "UserName": "user-name",
  "Email": "user@email.com",
  "Phone": "01715039303",
  "Gender": "male",
  "Dob": "01-01-2001",
  "PermanentAddress": "moylapota",
  "City": "khulna",
  "Country": "bangladesh",
  "IsActive": "INACTIVE",
  "IsSuperAdmin": "INACTIVE",
  "IsEmailVerified": "ACTIVE",
  "MFAType": "EMAIL",
  "IsMfa": "ACTIVE",
  "CreatedAt": "",
  "CreatedBy": "",
  "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
  "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Update profile Response example:

```json
{
  "Data": {
    "User": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Avatar": "avatar.jpg",
      "UserName": "user-name",
      "Email": "user@email.com",
      "Phone": "01715039303",
      "Gender": "male",
      "Dob": "01-01-2001",
      "PermanentAddress": "moylapota",
      "City": "khulna",
      "Country": "bangladesh",
      "IsActive": "INACTIVE",
      "IsSuperAdmin": "INACTIVE",
      "IsEmailVerified": "ACTIVE",
      "MFAType": "EMAIL",
      "IsMfa": "ACTIVE",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

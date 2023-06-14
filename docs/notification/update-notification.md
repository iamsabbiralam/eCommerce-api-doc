---
sidebar_position: 3
---

# Update

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can update a notification.

## 3. API

### Notification Create Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "UserID": "123e4567-e89b-12d3-a456-426614174000",
  "Type": "User create",
  "Title": "User create successfully",
  "Description": "User create successfully",
  "IsRead": 2,
  "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
  "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Notification Create Response example:

```json
{
  "Data": {
    "Notification": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "UserID": "123e4567-e89b-12d3-a456-426614174000",
      "Type": "User create",
      "Title": "User create successfully",
      "Description": "User create successfully",
      "IsRead": 2,
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

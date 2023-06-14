---
sidebar_position: 2
---

# Create

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce user can create a notification.

## 3. API

### Notification Create Request example:

```json
{
  "UserID": "123e4567-e89b-12d3-a456-426614174000",
  "Type": "User create",
  "Title": "User create successfully",
  "Description": "User create successfully",
  "IsRead": 1,
  "CreatedAt": "2020-03-24T06:03:00.348+03:00",
  "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Notification Create Response example:

```json
{
  "Data": {
    "Notification": {
      "ID": "123e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

---
sidebar_position: 3
---

# Update Setting

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can Update setting.

## 3. API

### Update Setting Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "Slug": "opt_code_update",
  "SettingGroup": "OTP",
  "Value": "12345678",
  "CreatedAt": "2020-03-24T06:03:00.348+03:00",
  "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Update Setting Response example:

```json
{
  "Data": {
    "Currency": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Slug": "opt_code_update",
      "SettingGroup": "OTP",
      "Value": "12345678",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

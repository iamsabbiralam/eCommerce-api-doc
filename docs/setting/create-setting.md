---
sidebar_position: 2
---

# Create Setting

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can add new setting.

## 3. API

### Create Setting Request example:

```json
{
  "Slug": "opt_code",
  "SettingGroup": "OTP",
  "Value": "12345678",
  "CreatedAt": "2020-03-24T06:03:00.348+03:00",
  "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Create Setting Response example:

```json
{
  "Data": {
    "Setting": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "Slug": "opt_code",
      "SettingGroup": "OTP",
      "Value": "12345678",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

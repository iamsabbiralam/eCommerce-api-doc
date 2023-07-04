---
sidebar_position: 9
---

# Get Sub Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-commerce admin can get details by ID or Name.

## 3. API

### Get Sub Category Request example:

```json
{
  "Name": "T-Shirt"
}
```

### Get Sub Category Response example:

```json
{
  "Data": {
    "SubCategory": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
      "Name": "T-Shirt",
      "IsActive": "1",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

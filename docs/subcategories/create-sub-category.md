---
sidebar_position: 8
---

# Create Sub Category

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce admin can add new sub category.

## 3. API

### Create Sub Category Request example:

```json
{
  "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
  "Name": "T-Shirt",
  "IsActive": "1",
  "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Create Sub Category Response example:

```json
{
  "Data": {
    "Category": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "CategoryID": "456e4567-e89b-12d3-a456-426614174000",
      "Name": "T-Shirt",
      "IsActive": "1",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```

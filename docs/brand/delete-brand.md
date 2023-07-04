---
sidebar_position: 5
---

# Delete Brand

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce system admin can delete brand by ID.


## 3. API

### Get Brand Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get Brand Response example:

```json
{
   "Data":{
      "Brand":{
            "IsDeleted": true
      }
   }
}
```
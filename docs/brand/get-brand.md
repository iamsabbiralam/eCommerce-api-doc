---
sidebar_position: 3
---

# Get Brand

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In e-Commerce system admin can get brand details by ID or Name.


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
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Name":"Easy",
         "Icon":"easy.png",
         "CreatedAt":"2023-03-24T06:03:00.348+03:00",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000",
         "UpdatedAt":"2023-03-24T06:03:00.348+03:00",
         "UpdatedBy":"456e4567-e89b-12d3-a456-426614174000"
      }
   }
}
```
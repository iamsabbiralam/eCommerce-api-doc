---
sidebar_position: 2
---

# Create Brand

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### #### In e-Commerce admin can create a brand.


## 3. API

### Create Brand Request example:

```json
{
   "Name":"Easy",
   "Icon":"easy.png",
   "Status":"ACTIVE",
}
```

### Create Brand Response example:

```json
{
   "Data":{
      "Brand":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Name":"Easy",
         "Icon":"easy.png",
         "Status":"ACTIVE",
         "CreatedAt":"2023-03-24T06:03:00.348+03:00",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000",
         "UpdatedAt":"2023-03-24T06:03:00.348+03:00",
         "UpdatedBy":"456e4567-e89b-12d3-a456-426614174000"
      }
   }
}
`
---
sidebar_position: 4
---

# Seller Profile

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

#### In e-commerce seller can view their profile.

## 3. API

### Seller Profile Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Seller Profile Response example:

```json
{
  "Data": {
    "Seller": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "StoreName": "Daraz",
      "Phone": "01715039303",
      "AccountType": "SellerAccount",
      "NidFrontSide": "nid.png",
      "NidBackSide": "nid.png",
      "NidName": "Sabbir",
      "NidNumber": "123456789101112131415",
      "BankStatement": "bank.jpg",
      "AccountName": "Sabbir",
      "BranchName": "Khulna",
      "AccountName": "164254845741",
      "Address": "Moylapota",
      "District": "Khulna",
      "Area": "Khulna",
      "State": "Khulna",
      "Country": "BD",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00"
    }
  }
}
```

---
sidebar_position: 1
---

# Brand Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A brand is a product, service or concept that is publicly distinguished from other products, services or concepts so that it can be easily communicated and usually marketed.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                                 | Description                                                      |
| ------------------------- | ------------ | ------------------------------------------- | ---------------------------------------------------------------- |
| id                        | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for brand                                      |
| icon                      | VARCHAR(100) | NOT NULL                                    | Icon for brand                                                   |
| name                      | VARCHAR(50)  | NOT NULL                                    | Brand name                                                       |
| status                    | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether brand status active or not               | 
| created_at                | DATETIME     | NOT NULL                                    | Timestamp when the brand was added                               |
| created_by                | UUID         | NOT NULL                                    | ID of admin who has added the brand                              |
| updated_at                | DATETIME     | NOT NULL                                    | Timestamp when the brand was last updated                        |
| updated_by                | UUID         | NOT NULL                                    | ID of admin who has updated the brand                            |
| deleted_at                | DATETIME     | NULL                                        | Timestamp when the brand was last deleted                        |
| deleted_by                | UUID         | NULL                                        | ID of admin who has deleted the brand                            |

`
`

## 4. Enum Fields

#### **status**

&nbsp;

    - STATUS_UNKNOWN
    - STATUS_ACTIVE
    - STATUS_INACTIVE
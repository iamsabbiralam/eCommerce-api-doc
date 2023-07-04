---
sidebar_position: 1
---

# Category Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

Category table holds information about the product category.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name | Data Type    | Constraints                                 | Description                                    |
| ---------- | ------------ | ------------------------------------------- | ---------------------------------------------- |
| id         | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for category                 |
| name       | VARCHAR(100) | NOT NULL, DEFAULT ""                        | Unique identifier for category name            |
| is_active  | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether the category is active |
| created_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the role was created            |
| created_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has created the role           |
| updated_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the role was last updated       |
| updated_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the role           |
| deleted_at | DATETIME     | NULL                                        | Timestamp when the role was last deleted       |
| deleted_by | UUID         | NULL                                        | ID of admin who has deleted the role           |

## 4. Enum Fields

#### **IsActive**

&nbsp;

    - IS_ACTIVE_TRUE
    - IS_ACTIVE_FALSE

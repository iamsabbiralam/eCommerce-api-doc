---
sidebar_position: 3
---

# User Address Overview

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

User address is a common component of a database that is used to store information about users address or individuals in a system.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name | Data Type    | Constraints                                 | Description                                    |
| ---------- | ------------ | ------------------------------------------- | ---------------------------------------------- |
| id         | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for user address             |
| user_id    | UUID         | UUID FOREIGN KEY                            | Unique identifier for user                     |
| address    | VARCHAR(150) | NOT NULL, DEFAULT ""                        | Address identifier for user                    |
| city       | VARCHAR(50)  | NOT NULL, DEFAULT ""                        | City identifier for user                       |
| country    | VARCHAR(50)  | NOT NULL, DEFAULT ""                        | Country identifier for user                    |
| is_default | BOOLEAN      | NOT NULL, DEFAULT FALSE                     | is_default identifier for user default address |
| created_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was added              |
| created_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has added the user             |
| updated_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was last updated       |
| updated_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the user           |
| deleted_at | DATETIME     | NULL                                        | Timestamp when the user was last deleted       |
| deleted_by | UUID         | NULL                                        | ID of admin who has deleted the user           |

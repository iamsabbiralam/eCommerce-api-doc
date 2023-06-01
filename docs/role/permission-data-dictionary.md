---
sidebar_position: 2
---

# Permission Overview

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

Role permission table, also known as an access control matrix, is a tool used to define and manage permissions within a system or organization.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name | Data Type    | Constraints                                 | Description                              |
| ---------- | ------------ | ------------------------------------------- | ---------------------------------------- |
| id         | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for permission         |
| role_id    | UUID         | UUID DEFAULT FOREIGN KEY                    | Unique identifier for role               |
| name       | VARCHAR(100) | NOT NULL, DEFAULT ""                        | Unique identifier for permission         |
| resource   | TEXT         | NULL, DEFAULT ""                            | Resource hold the group of module name   |
| action     | VARCHAR(255) | NULL , DEFAULT []                           | Access name of the modules               |
| created_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was added        |
| created_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has added the user       |
| updated_at | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was last updated |
| updated_by | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the user     |
| deleted_at | DATETIME     | NULL                                        | Timestamp when the user was last deleted |
| deleted_by | UUID         | NULL                                        | ID of admin who has deleted the user     |

---
sidebar_position: 1
---

# Setting Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

In the context of a project, a setting table refers to a table or data structure that is used to organize and store data or information related to the project.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name    | Data Type    | Constraints                                 | Description                                 |
| ------------- | ------------ | ------------------------------------------- | ------------------------------------------- |
| id            | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for setting               |
| slug          | VARCHAR(100) | NOT NULL, UNIQUE                            | Unique identifier for setting slug          |
| setting_group | TEXT         | NOT NULL, DEFAULT ""                        | Setting Group                               |
| value         | TEXT         | NOT NULL, DEFAULT ""                        | Value of setting                            |
| created_at    | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the setting was created      |
| created_by    | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has created the setting     |
| updated_at    | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the setting was last updated |
| updated_by    | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the setting     |

---
sidebar_position: 3
---

# User Role Overview

## 1. version control

| Version        | Date          | Description of Changes |
| -------------- | ------------- | ---------------------- |
| eCommerce V1.0 | June 01, 2023 | Initial Release        |

## 2. Overview

User role table, also known as a role-based access control (RBAC) table, is a tool used to define and manage the roles assigned to individual users within a system or organization.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name | Data Type | Constraints                                 | Description                                   |
| ---------- | --------- | ------------------------------------------- | --------------------------------------------- |
| id         | UUID      | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for permission              |
| user_id    | UUID      | UUID DEFAULT FOREIGN KEY                    | Unique identifier for user                    |
| role_id    | UUID      | UUID DEFAULT FOREIGN KEY                    | Unique identifier for role                    |
| created_at | DATETIME  | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user role was added        |
| created_by | UUID      | NOT NULL, DEFAULT ""                        | ID of admin who has added the user role       |
| updated_at | DATETIME  | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user role was last updated |
| updated_by | UUID      | NOT NULL, DEFAULT ""                        | ID of admin who has updated the user role     |
| deleted_at | DATETIME  | NULL                                        | Timestamp when the user role was last deleted |
| deleted_by | UUID      | NULL                                        | ID of admin who has deleted the user role     |

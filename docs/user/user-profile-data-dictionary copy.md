---
sidebar_position: 2
---

# User Profile Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

User Profile table is a common component of a database that is used to store information about users or individuals in a system. It typically represents a collection of records, with each record representing a specific user.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name        | Data Type    | Constraints                                 | Description                              |
| ----------------- | ------------ | ------------------------------------------- | ---------------------------------------- |
| id                | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for user profile       |
| user_id           | UUID         | UUID DEFAULT FOREIGN KEY                    | Unique identifier for user               |
| first_name        | VARCHAR(50)  | NULL, DEFAULT ""                            | Unique identifier for user's first name  |
| last_name         | VARCHAR(50)  | NULL , DEFAULT ""                           | Unique identifier for user's last name   |
| phone             | VARCHAR(20)  | NULL, UNIQUE , DEFAULT ""                   | Unique identifier for user's phone       |
| gender            | VARCHAR(10)  | NULL , DEFAULT ""                           | gender of a user                         |
| dob               | DATE         | NULL                                        | date of birth of a user                  |
| permanent_address | VARCHAR(150) | NULL , DEFAULT ""                           | permanent address of a user              |
| city              | VARCHAR(50)  | NULL , DEFAULT ""                           | city of a user                           |
| country           | VARCHAR(50)  | NULL , DEFAULT ""                           | country name of a user                   |
| created_at        | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was added        |
| created_by        | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has added the user       |
| updated_at        | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was last updated |
| updated_by        | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the user     |
| deleted_at        | DATETIME     | NULL                                        | Timestamp when the user was last deleted |
| deleted_by        | UUID         | NULL                                        | ID of admin who has deleted the user     |

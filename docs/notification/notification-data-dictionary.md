---
sidebar_position: 1
---

# Notification Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

Notification table represents a basic structure for managing notifications in a system.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name  | Data Type    | Constraints                                 | Description                                         |
| ----------- | ------------ | ------------------------------------------- | --------------------------------------------------- |
| id          | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for notification                  |
| user_id     | UUID         | UUID DEFAULT FOREIGN KEY                    | Unique identifier for notification                  |
| type        | VARCHAR(50)  | NOT NULL, DEFAULT ""                        | Identifier for notification type                    |
| title       | VARCHAR(255) | NOT NULL, DEFAULT ""                        | Identifier for notification title                   |
| description | TEXT         | NOT NULL, DEFAULT ""                        | Description for notification                        |
| is_read     | tinyint(1)   | DEFAULT 0                                   | Is read indicating whether the notification is read |
| created_at  | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the notification was added           |
| created_by  | UUID         | NOT NULL, DEFAULT ""                        | ID of user who has added the notification           |
| updated_at  | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the notification was last updated    |
| updated_by  | UUID         | NOT NULL, DEFAULT ""                        | ID of user who has updated the notification         |
| deleted_at  | DATETIME     | NULL                                        | Timestamp when the notification was last deleted    |
| deleted_by  | UUID         | NULL                                        | ID of user who has deleted the notification         |

## 4. Enum Fields

#### **IsRead**

&nbsp;

    - IS_READ_TRUE
    - IS_READ_FALSE

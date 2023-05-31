---
sidebar_position: 1
---

# User Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

User table is a common component of a database that is used to store information about users or individuals in a system. It typically represents a collection of records, with each record representing a specific user.

## 3. Data Dictionary (eCommerce V1.0)

| Field Name        | Data Type    | Constraints                                 | Description                                                    |
| ----------------- | ------------ | ------------------------------------------- | -------------------------------------------------------------- |
| id                | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for user                                     |
| avatar            | VARCHAR(100) | NOT NULL, DEFAULT ""                        | Image for user                                                 |
| username          | VARCHAR(50)  | NOT NULL, UNIQUE                            | Unique identifier for user                                     |
| email             | VARCHAR(100) | NOT NULL, UNIQUE                            | Unique identifier for user                                     |
| password          | VARCHAR(15)  | NOT NULL                                    | Password for user                                              |
| is_active         | tinyint(1)   | DEFAULT 0                                   | Is active indicating whether the user is active                |
| is_super_admin    | tinyint(1)   | DEFAULT 0                                   | Is super admin indicating whether the user is admin            |
| is_email_verified | tinyint(1)   | DEFAULT 0                                   | Is email verified indicating whether the user is verified      |
| mfa_type          | VARCHAR(20)  | NULL, DEFAULT ""                            | Mfa type indicating whether the user is authenticated by email |
| is_mfa            | tinyint(1)   | DEFAULT 0                                   | Is mfa indicating whether the user is verified                 |
| created_at        | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was added                              |
| created_by        | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has added the user                             |
| updated_at        | DATETIME     | NOT NULL, DEFAULT current_timestamp         | Timestamp when the user was last updated                       |
| updated_by        | UUID         | NOT NULL, DEFAULT ""                        | ID of admin who has updated the user                           |
| deleted_at        | DATETIME     | NULL                                        | Timestamp when the user was last deleted                       |
| deleted_by        | UUID         | NULL                                        | ID of admin who has deleted the user                           |

## 4. Enum Fields

#### **MfaType**

&nbsp;

    - MFA_TYPE_UNKNOWN
    - MFA_TYPE_EMAIL
    - MFA_TYPE_OTP

#### **IsSuperAdmin**

&nbsp;

    - IS_SUPER_ADMIN_UNKNOWN
    - IS_SUPER_ADMIN_ACTIVE
    - IS_SUPER_ADMIN_INACTIVE

#### **IsEmailVerified**

&nbsp;

    - IS_EMAIL_VERIFIED_UNKNOWN
    - IS_EMAIL_VERIFIED_ACTIVE
    - IS_EMAIL_VERIFIED_INACTIVE

#### **IsMFA**

&nbsp;

    - IS_MFA_UNKNOWN
    - IS_MFA_EMAIL
    - IS_MFA_OTP

#### **IsActive**

&nbsp;

    - IS_ACTIVE_TRUE
    - IS_ACTIVE_FALSE

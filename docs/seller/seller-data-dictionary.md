---
sidebar_position: 1
---

# Seller Overview

## 1. version control

| Version        | Date         | Description of Changes |
| -------------- | ------------ | ---------------------- |
| eCommerce V1.0 | May 31, 2023 | Initial Release        |

## 2. Overview

## 3. Data Dictionary Seller(eCommerce V1.0)

| Field Name        | Data Type    | Constraints                                 | Description                                           |
| ----------------- | ------------ | ------------------------------------------- | ----------------------------------------------------- |
| id                | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for seller                          |
| email             | VARCHAR(100) | NOT NULL,UNIQUE                             | Unique identifier for seller, seller email            |
| password          | VARCHAR(50)  | NOT NULL                                    | Password for seller                                   |
| is_active         | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether seller active or not          |
| is_email_verified | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether seller verified through email |
| approval_status   | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether seller approvide by admin     |
| business_address  | UUID         | UUID DEFAULT uuid_generate_v4()             | Seller business address id                            |
| created_at        | DATETIME     | NOT NULL                                    | Timestamp when the seller was added                   |
| created_by        | UUID         | NOT NULL                                    | ID of admin who has added the seller                  |
| updated_at        | DATETIME     | NULL                                        | Timestamp when the seller was last updated            |
| updated_by        | UUID         | NOT NULL                                    | ID of admin who has updated the seller                |
| deleted_at        | DATETIME     | NULL                                        | Timestamp when the seller was last delete             |
| deleted_by        | UUID         | NOT NULL                                    | ID of admin who has delete the seller                 |

## 4. Data Dictionary Seller_address(eCommerce V1.0)

| Field Name       | Data Type    | Constraints                                 | Description                                  |
| ---------------- | ------------ | ------------------------------------------- | -------------------------------------------- |
| id               | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for seller address         |
| seller_id        | UUID         | UUID DEFAULT uuid_generate_v4() Foren KEY   | Unique identifier for seller                 |
| country          | VARCHAR(100) | NOT NULL                                    | Seller country                               |
| state            | VARCHAR(100) | NOT NULL                                    | Seller state                                 |
| area             | VARCHAR(100) | NOT NULL                                    | Seller leaving area                          |
| district         | VARCHAR(100) | NOT NULL                                    | Seller disteic                               |
| business_address | VARCHAR(100) | NOT NULL                                    | Seller business address                      |
| created_at       | DATETIME     | NOT NULL                                    | Timestamp when the currency was added        |
| created_by       | UUID         | NOT NULL                                    | ID of admin who has added the currency       |
| updated_at       | DATETIME     | NOT NULL                                    | Timestamp when the currency was last updated |
| updated_by       | UUID         | NOT NULL                                    | ID of admin who has updated the currency     |

## 5. Data Dictionary Seller_Information(eCommerce V1.0)

| Field Name     | Data Type    | Constraints                                 | Description                                      |
| -------------- | ------------ | ------------------------------------------- | ------------------------------------------------ |
| id             | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for seller address             |
| seller_id      | UUID         | UUID DEFAULT uuid_generate_v4() Foren KEY   | Unique identifier for seller                     |
| store_name     | VARCHAR(100) | NOT NULL                                    | Seller store name                                |
| phone          | VARCHAR(100) | NOT NULL                                    | Seller phone number                              |
| account_type   | VARCHAR(100) | NOT NULL                                    |                                                  |
| nid_front_side | VARCHAR(300) | NOT NULL                                    | Seller national identity card front side picture |
| nid_back_side  | VARCHAR(300) | NOT NULL                                    | Seller national identity card back side picture  |
| nid_name       | VARCHAR(100) | NOT NULL                                    | Seller name in national identity card            |
| nid_number     | VARCHAR(100) | NOT NULL                                    | seller national identity card number             |
| bank_statement | VARCHAR(100) | NOT NULL                                    | seller bank statement                            |
| account_name   | VARCHAR(100) | NOT NULL                                    | seller bank account name                         |
| bank_name      | VARCHAR(100) | NOT NULL                                    | seller bank name                                 |
| branch_name    | VARCHAR(100) | NOT NULL                                    | seller bank accout branch                        |
| account_number | VARCHAR(100) | NOT NULL                                    | seller bank account number                       |
| created_at     | DATETIME     | NOT NULL                                    | Timestamp when the seller was added              |
| created_by     | UUID         | NULL                                        | ID of admin who has added the seller             |
| updated_at     | DATETIME     | NOT NULL                                    | Timestamp when the seller was last updated       |
| updated_by     | UUID         | NOT NULL                                    | ID of admin who has updated the seller           |
| deleted_at     | DATETIME     | NULL                                        | Timestamp when the seller was last updated       |
| deleted_by     | UUID         | NOT NULL                                    | ID of admin who has updated the seller           |


## 6. Enum Fields

#### _CoinType_

&nbsp;

    - COIN_TYPE_UNKNOWN
    - COIN_TYPE_FIAT
    - COIN_TYPE_CRYPTO

#### _ExchangeStatus_

&nbsp;

    - EXCHANGE_STATUS_UNKNOWN
    - EXCHANGE_STATUS_ACTIVE
    - EXCHANGE_STATUS_INACTIVE

#### _DepositStatus_

&nbsp;

    - DEPOSIT_STATUS_UNKNOWN
    - DEPOSIT_STATUS_ACTIVE
    - DEPOSIT_STATUS_INACTIVE

#### _WithdrawalStatus_

&nbsp;

    - WITHDRAWAL_STATUS_UNKNOWN
    - WITHDRAWAL_STATUS_ACTIVE
    - WITHDRAWAL_STATUS_INACTIVE

#### _IsActive_

&nbsp;

    - IS_ACTIVE_TRUE
    - IS_ACTIVE_FALSE

#### _DepositFeeType_

&nbsp;

    - DEPOSIT_FEE_TYPE_UNKNOWN
    - DEPOSIT_FEE_TYPE_FEE_TYPE_FIXED
    - DEPOSIT_FEE_TYPE_FEE_TYPE_PERCENTAGE

#### _WithdrawalFeeType_

&nbsp;

    - WITHDRAWAL_FEE_TYPE_UNKNOWN
    - WITHDRAWAL_FEE_TYPE_FEE_TYPE_FIXED
    - WITHDRAWAL_FEE_TYPE_FEE_TYPE_PERCENTAGE

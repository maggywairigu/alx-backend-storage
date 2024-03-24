# Project: MySQL Advanced

## Overview

This project focuses on advanced MySQL concepts and practices, including creating tables with constraints, optimizing queries with indexes, implementing stored procedures, functions, views, and triggers. It consists of several tasks, each requiring the creation of SQL scripts to perform specific database operations.

## Resources

Before starting the tasks, you may want to review the following resources:

- [MySQL cheatsheet](#)
- [MySQL Performance: How To Leverage MySQL Database Indexing](#)
- [Stored Procedure](#)
- [Triggers](#)
- [Views](#)
- [Functions and Operators](#)
- [Trigger Syntax and Examples](#)
- [CREATE TABLE Statement](#)
- [CREATE PROCEDURE and CREATE FUNCTION Statements](#)
- [CREATE INDEX Statement](#)
- [CREATE VIEW Statement](#)

## Learning Objectives

Upon completing this project, you should be able to:

- Create tables with constraints
- Optimize queries by adding indexes
- Implement stored procedures and functions in MySQL
- Implement views and triggers in MySQL

## Requirements

General requirements for the project include:

- Files to be executed on Ubuntu 18.04 LTS using MySQL 5.7 (version 5.7.30)
- All files should end with a new line
- All SQL queries should have a comment just before
- All files should start with a comment describing the task
- All SQL keywords should be in uppercase (SELECT, WHERE, etc.)
- A README.md file at the root of the folder of the project is mandatory

## Tasks

### Task 0: We are all unique!
- Create a table `users` with specified attributes
- Ensure uniqueness of the email attribute
- If the table already exists, the script should not fail

### Task 1: In and not out
- Create a table `users` with specified attributes, including an enumeration for country
- Default country should be US
- If the table already exists, the script should not fail

### Task 2: Best band ever!
- Rank country origins of bands based on the number of fans
- Import table dump `metal_bands.sql`

### Task 3: Old school band
- List bands with Glam rock as their main style, ranked by their longevity
- Import table dump `metal_bands.sql`

### Task 4: Buy buy buy
- Create a trigger to decrease the quantity of an item after adding a new order

### Task 5: Email validation to sent
- Create a trigger to reset the attribute `valid_email` when the email has been changed

### Task 6: Add bonus
- Create a stored procedure `AddBonus` to add a new correction for a student

### Task 7: Average score
- Create a stored procedure `ComputeAverageScoreForUser` to compute and store the average score for a student

### Task 8: Optimize simple search
- Create an index on the table `names` for the first letter of the name

### Task 9: Optimize search and score
- Create an index on the table `names` for the first letter of the name and the score

### Task 10: Safe divide
- Create a function `SafeDiv` to divide two numbers safely

### Task 11: No table for a meeting
- Create a view `need_meeting` to list students with scores under 80 and no last meeting or more than 1 month

## Directory Structure

```
alx-backend-storage/
│
└── 0x00-MySQL_Advanced/
    ├── README.md
    ├── 0-uniq_users.sql
    ├── 1-country_users.sql
    ├── 2-fans.sql
    ├── 3-glam_rock.sql
    ├── 4-init.sql
    ├── 4-store.sql
    ├── 4-main.sql
    ├── 5-init.sql
    ├── 5-valid_email.sql
    ├── 5-main.sql
    ├── 6-init.sql
    ├── 6-bonus.sql
    ├── 6-main.sql
    ├── 7-init.sql
    ├── 7-average_score.sql
    ├── 7-main.sql
    ├── 8-index_my_names.sql
    ├── 9-index_name_score.sql
    ├── 10-init.sql
    ├── 10-div.sql
    ├── 11-init.sql
    ├── 11-need_meeting.sql
    └── 11-main.sql
```

## Running the Scripts

1. Ensure MySQL 5.7 is installed and running on Ubuntu 18.04 LTS.
2. Execute each SQL script in the corresponding task.
3. Review the output and ensure the desired database modifications are made.

Enjoy MySQL advanced concepts and practices!
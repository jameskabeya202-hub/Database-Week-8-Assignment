-- Week 8 Assignment: MySQL Database Backup and Restore

-- Question 1: Creating a Complete Database Backup
-- Run this command in Command Prompt or PowerShell.
-- It prompts for the root password and saves the sales database structure and data
-- to sales_backup.sql. Regular backups help recover from accidental changes,
-- hardware failure, corruption, or other data loss.
mysqldump -u root -p --databases sales --result-file=sales_backup.sql


-- Question 2: Backing Up All Databases
-- Run this command in Command Prompt or PowerShell.
-- It prompts for the root password and exports every database on the server
-- to all_databases_backup.sql. This helps preserve the databases and their data
-- when migrating to another server.
mysqldump -u root -p --all-databases --result-file=all_databases_backup.sql

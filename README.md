# Student Database Project

This repository contains the necessary SQL scripts to set up a student database management system using MySQL.
It includes scripts to create a database, tables, insert data, and perform some basic queries and data manipulation.

## Prerequisites

Before you begin, ensure you have the follwing installed:
- MySQL Server
- Bash Shell (Unix/Linux/MacOS)

This script has been tested on Ubuntu 20.04. If you are using another operating system, you might need to adjust the instalation commands and procedures accordingly in the run_script.sh file.

## Installation and Setup

1. **Clone the Repository**
Start by cloning this repository to your local machine. To do so, run the following commands in your terminal:

```bash
git clone https://github.com/AnanGharra/StudentDB
cd StudentDB
```

2. **Change permission for the run script file**

```bash
chmod +x run_script.sh
```

3. **Run the script file**

```bash
./run_script.sh
```

## Usage
This script will:
- Install MySQL Server if it is not already installed.
- Start the MySQL service.
- Create a database and tables.
- Insert initial data.
- Run predefined queries and data manipulations.
**Note:** The script might prompt for your root's password for installation purposes and MySQL's root password to access the database.

## Manual Setup
If you prefer to setup the database manually, you can run the SQL scripts directly in your MySQL client:

```sql
SOURCE path/to/create_table.sql;
SOURCE path/to/insert_data.sql;
SOURCE path/to/queries.sql; --Optional
SOURCE path/to/data_manipulation.sql; --Optional
```

## Troublshooting
If you encounter the "Access denied for user 'root'@'localhost'" error, it may be due to MySQL being configured to authenticate the 'root' user via the 'auth_socket' plugin. See the official MySQL documentation for guidance on changing authenrication methods or using 'sudo' to access MySQL.



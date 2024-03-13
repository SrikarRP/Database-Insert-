# Python Program to Import Data from CSV into SQL Server

This Python program demonstrates how to import data from a CSV file into a SQL Server database using the pyodbc library.

## Installation

Before running the program, make sure you have the following libraries installed:

- pyodbc
- csv

You can install them using pip:

```bash
pip install pyodbc
Usage
1.Replace the connection details (server, database, username, password) with your actual credentials.
2.Specify the path to your CSV file (csv_file).
3.Run the Python program.
```

#Different drivers for different DBs
```
ODBC Driver for SQL Server:

ODBC Driver 17 for SQL Server: This is Microsoft's ODBC driver for SQL Server.
SQL Server Native Client: An older Microsoft ODBC driver for SQL Server, now deprecated in favor of ODBC Driver 17.
ODBC Driver for MySQL:

MySQL ODBC Connector: Provided by MySQL, this driver allows you to connect to MySQL databases.
ODBC Driver for PostgreSQL:

PostgreSQL ODBC Driver: Allows you to connect to PostgreSQL databases.
ODBC Driver for Oracle:

Oracle ODBC Driver: Provided by Oracle, this driver allows you to connect to Oracle databases.
ODBC Driver for SQLite:

SQLite ODBC Driver: This driver allows you to connect to SQLite databases.
ODBC Driver for IBM Db2:

IBM Db2 ODBC Driver: Enables connections to IBM Db2 databases.
ODBC Driver for MariaDB:

MariaDB ODBC Connector: Allows you to connect to MariaDB databases.
ODBC Driver for Amazon Redshift:

Amazon Redshift ODBC Driver: Enables connections to Amazon Redshift data warehouses.
```
This project is licensed under the MIT License - see the LICENSE file for details.


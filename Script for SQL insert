# %%
import csv
import pyodbc

# Connection details (replace with your actual credentials)
server = "SRIKAR\SQLSRI2024"
database = "Test"
username = "sa"
password = "srikar"

# Connect to the database
conn_string = f"DRIVER={{ODBC Driver 17 for SQL Server}};SERVER={server};DATABASE={database};UID={username};PWD={password}"
conn = pyodbc.connect(conn_string)
cursor = conn.cursor()

# CSV file path (replace with your actual file path)
csv_file = "C:/Users/srika/Downloads/username.csv"

# Open the CSV file
with open(csv_file, 'r') as file:
    reader = csv.reader(file, delimiter=';')  # Specify the delimiter

    # Skip the header row (if present)
    next(reader)

    # Iterate through each row and insert data
    for row in reader:
        try:
            # Removed the empty brackets
            insert_statement = "INSERT INTO dbo.username VALUES (?, ?, ?, ?)"
            values = row
            print(f"Executing statement: {insert_statement} with values: {values}")
            cursor.execute(insert_statement, values)
        except pyodbc.Error as ex:
            print("Error inserting row:", row)
            print("Error details:", ex)

# Commit changes and close connection
conn.commit()
cursor.close()
conn.close()

print("CSV data imported successfully!")




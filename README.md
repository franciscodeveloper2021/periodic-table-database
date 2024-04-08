# Periodic Table Database

This repository contains a PostgreSQL database dump for a periodic table database along with a Bash script for interacting with the database.

## Files

- **periodic_table_dump.sql**: This file contains the SQL dump of the PostgreSQL database. It includes tables for elements, properties, and types, along with constraints and sample data.

- **periodic_table_script.sh**: This Bash script provides functions for querying and updating the periodic table database. It includes functions for printing element information, fixing database issues, and starting the main program.

## Usage

1. **Clone the Repository**: Clone this repository to your local machine using the following command:
```
git clone https://github.com/your-username/periodic-table-database.git
```

2. **Import the Database**: Import the SQL dump file into your PostgreSQL database using a tool like `pg_restore` or `psql`:
```
 pg_restore -U username -d database_name periodic_table_dump.sql
```

3. **Execute the Bash Script**: Run the Bash script to interact with the database:
```
./periodic_table_script.sh
```

## Functionality

- **Query Elements**: You can query element information by providing either the element symbol or atomic number as an argument to the script.
```
./periodic_table_script.sh H
./periodic_table_script.sh 1
```

- **Fix Database**: The script includes a function to fix database issues, such as renaming columns, adding constraints, and inserting missing elements.
```
./periodic_table_script.sh fix
```

- **Main Program**: The script's main program prompts the user to input an element and displays its information.
```
./periodic_table_script.sh
```

## License

This project is licensed under the [MIT License](LICENSE).

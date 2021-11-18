# Use bulk insert to load data

1. Prerequisites
   * run steps 1 & 2 from `01 Create a MIMIC database`
   * Extract all MIMIC-III *.csv.gz files to *.csv
1. Open `mimic3-load.sql`
   1. Replace `/path/to/data/` with path to CSV files (files must be extracted from gz)
   1. Run
1. Continue with other steps as needed

# Original instructions from https://github.com/SpiroGanas/MIMIC-on-SQL-Server to load data using SSIS

This folder contains a SQL Server 2016 SSIS package.  This SSIS package will load the un-zipped MIMIC III CSV Files into the SQL Server tables.

You can open this SSIS package using SQL Server Data Tools:  https://docs.microsoft.com/en-us/sql/ssdt/download-sql-server-data-tools-ssdt

The SSIS package contains three parameters, which you can set to point to the folder containing the CSV files and the database on your SQL Server.

To download the MIMIC III CSV files, follow the instructions here: https://mimic.physionet.org/gettingstarted/access/
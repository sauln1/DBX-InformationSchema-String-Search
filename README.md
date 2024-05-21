# DBX-InformationSchema-String-Search
A databricks notebook designed to search for a string in every column and table in a catalog.

# InformationSchema String Search
This script is designed to use the information schema in Databricks catalog and search all columns in all available tables for a string. In order to run a search:
1. Enter the desired schema and, if you only want to search all columns in a single table, the table name. These are used in a 'LIKE' search, so approximate names are allowed. You can leave both of these blank to search every schema and every table.
2. Enter the string you want to search for. You can add in %% surrounding the string within the quotes to use a 'LIKE' search if you don't know the exact string.
Any matching table columns will be output after the script is run.

#### WARNING: Depending on how large the catalog and target schema is, this may take a lot of time and compute resources.

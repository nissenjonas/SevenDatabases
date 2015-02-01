#PostgreSQL
##Links
- [PostgreSQL FAQ](https://wiki.postgresql.org/wiki/FAQ)
##psql 
PostgreSQL interactive terminal

###Connect to database with psql shell
	psql [database]
	
	# e.g.
	psql book

###psql commands
	\q 						# Quit	
	\di						# Lists all indexes on a database
	\h 						# Lists all SQL commands
	\h CREATE INDEX 		# SQL Command specific help
	\? 						# List all psql commands

###psql script
	# Example script connects to book database and executes command (-c) to create table countries
	psql book -c "create table countries(
							country_code char(2) Primary Key,
							country_name text UNIQUE
						);"

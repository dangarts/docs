# PostgreSQL
An interactive command line interface for executing SQL code
Best results install Postgres via Homebrew.

## Terminal
`psql` login to postgres via terminal
`createdb` 
`psql -h localhost` 
`psql -f path-of-file.sql name-of db-to-create <username>` import
`psql db-name-created <username>` enter into db to start querying data

## PSQL
- `\?` for help with psql commands
- `\l` or `\list` list all db information
- `\l` or `\list` list all db information
- `\q` quit psql
- `\h` for help with SQL commands
- `\s` - Command history
- `\s filename` - Save command history to file
- `\i filename` - Execute psql commands from a file
- `\?` - psql commands
- `\h <command-name>` - for specific details on the command
- `\q` - quit postgres

---

- `psql -d database -U  user -W` - connecting general
- `psql -h host -d database -U user -W` - connecting to a host
- `psql -U user -h host "dbname=db sslmode=require"` - connecting ssl mode
- `\c dbname username` -  Switch Connection to a new database
- `\l` - List available databases
- `\dt` - List available tables
- `\d table_name` - Describe a table
- `\dn` - List available schema [on currently connected database]
- `\df` - List available functions 
- `\dv` - List available views [on connected db]
- `\du` - List all user and their roles

### Execute the previous command
   - `SELECT version();` - retrieve current version
   - `\g` - executes the previous command
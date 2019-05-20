# PostgreSQL
An interactive command line interface for executing SQL code
Best results install Postgres via Homebrew.

## Terminal
- `psql` login to postgres via terminal
- `createdb` 
- `psql -h localhost` 
- `psql -f path-of-file.sql name-of db-to-create <username>` import
- `psql db-name-created <username>` enter into db to start querying data

## Start/Stop/Restart Postgres

- `pg_ctl -D /usr/local/var/postgres[VERSION NUMBER HERE] start`
- `pg_ctl -D /usr/local/var/postgres[VERSION NUMBER HERE] stop`
- `brew services list`
- `brew services restart postgresql`
- `brew services start postgresql`
- `brew services stop postgresql`

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

### Sequelize to model data
- start postgres 
  - `pg_ctl -D /usr/local/var/postgres[VERSION NUMBER HERE] start`
- create database(s) 
  - createdb -U postgres -w db-name-dev-or-test
- add the modules needed for the database and ORM
  - `npm i --save sequelize@4.32.6 pg@7.4.1 pg-hstore@2.3.2`
- Sequelize CLI
  - `npm i -g sequelize-cli@4.0.0`
- create our Sequelize configuration file
  - `touch .sequelizerc` add data to that file
- run the config file
  - `sequelize init`
- edit/review `src/db/config/config.json`

### Heroku DB access

- `heroku psql`
- `heroku run sequelize db:migrate:undo:all`
- `heroku run sequelize db:migrate`


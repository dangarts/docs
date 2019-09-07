### Heroku DB access

- `heroku psql`
- `heroku run sequelize db:migrate:undo:all`
- `heroku run sequelize db:migrate`

- `sequelize seed:generate --name user` create a seed file named queries.users.js
- `sequelize db:seed:all` seed all

### Sequelize ###

- `sequelize db:migrate:undo:all && sequelize db:migrate:undo:all --env test`
- `sequelize db:migrate && sequelize db:migrate --env test`
- `heroku run sequelize db:migrate`
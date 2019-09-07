# Server

- Pushing secrets to remote server
  - `heroku config:set megasecret="but there are plenty of forks"`

# Node Processes

- list all Node process

  - `ps -e|grep node`

- how many nodejs processes running

  - `ps -aef | grep node`

- Kill specific process

  - `kill -9 XXXX`

- Kill all processes
  - `pkill node`

# nginx

- test scripts

  - `sudo nginx -t`

- reload config

  - `sudo nginx -s reload`

- restart
  - `sudo service nginx restart`

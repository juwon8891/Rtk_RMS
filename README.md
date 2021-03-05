# WebOS RTK Admin

## How to setup development environment

* Prerequisite
  * nodejs
  * docker / docker-compose

1. Clone this repository with submodule include
  * `git clone --recurse-submodules ${repository_uri}`
2. Create .env
  * you can refer .env.template
3. Run docker-compose to setup db, reverse proxy and other utility services
  * `docker-compose -f docker-compose.dev.yml up -d`
4. Run backend server
  * go to services/backend
  * create .env (check README.md)
  * `yarn start`
5. Run frontend
  * go to services/frontend
  * create .env (check README.md)
  * `yarn serve`
6. You can access via http://localhost
  * frontend: http://localhost/
  * apidocs: http://localhost/api/v1/docs
  * express: http://localhost/express
  * agendash: http://localhost/agendash

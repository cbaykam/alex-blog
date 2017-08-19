## Test project
 This project is built as a `Test Task` only

## Requirements
- Docker & docker-compose
- git

## Installation
- Clone the repository
- Install submodules to get the docker container configuration. `git pull --recurse-submodules`
- change the line 36 in the laradoc/.env to `WORKSPACE_INSTALL_NODE=true`
- copy .env.example to .env
- launch the containers `docker-compose up -d nginx mysql`
- `docker-compose exec workspace bash` to get in the main container.
- Run the migrations `php artisan migrate`
- `npm install`
- You're all set.

## Development
- To run shell commands in the Laravel container. `docker-compose exec workspace bash`
- To watch changes `yarn run watch`


## Compiling assets
-

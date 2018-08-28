# Docker Rails 5 Boilerplate

The intent of this boilerplate is to serve as example for Rails 4 projects created from scratch using Docker.

## Pre-requisites

1. Have docker installed
2. Have the preferable IDE installed to edit files
3. Have docker running

## How to use this files?

1. Copy Dockerfile, Gemfile and docker-compose.yml to a new folder where you want to create the Rails project
2. Run, inside the folder, the command `docker-compose build`
3. Now create the Rails app using `docker-compose run bundle exec rails new . --force --database=postgresql --skip-bundle`
4. Run build again `docker-compose build` to install the Gems
5. After that you do normal Rails' tasks and commands using `docker-compose run rails bin/rails ...`

## Editing `credentials.yml.enc` file

1. Start the container with `docker-compose up`
2. Run the edit with ``

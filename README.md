# README

## Setup Docker for Rails/PostgreSQL app

Flow instructions: https://docs.docker.com/samples/rails/

## Create crud app with scaffold

```powershell
  docker-compose run --rm web rails g scaffold Task title:string description:text status:decimal
  docker-compose run --rm web rake db:migrate
```

## Run app

```powershell
  docker-compose up
```

Link running app: http://localhost:3000/tasks

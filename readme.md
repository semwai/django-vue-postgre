 backend

 `docker-compose run web django-admin startproject base server `

 frontend

 `docker-compose run client vue init webpack-simple .`

## Usage

 `docker-compose up`

## Problem

The django server starts up at the same time as the database starts. The database is not available and the server cannot receive a connection. Solution: reboot the server container. 

`docker ps`

find like `81a2b461765e   django-vue-postgre_server` and

`docker restart 81a2b461765e`
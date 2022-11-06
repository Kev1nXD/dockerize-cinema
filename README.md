# Cinema API

API service for cinema management written on DRF  

## Installation

Python3, is required

```shell
git clone https://github.com/Kev1nXD/dockerize-cinema.git
python3 -m venv venv
source venv/bin/activate (Linux)
venv\Scripts\activate (Windows)
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db user password>
python manage.py migrate
python manage.py runserver
```

## Run with docker

Docker is required
```shell
docker-compose build
docker-compose up
```
After all you will be able to connect to API on your localhost (127.0.0.1:8000)

## Getting access
* create user via /api/user/register/
* get access (tokens) via /api/user/token/

## Features

* JWT authenticated
* Admin panel /admin/
* Documentation is located at api/dac/swagger/
* Managing orders and tickets
* Creating movie with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions

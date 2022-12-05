cinema-api-docker
A simple service providing REST API for a cinema. Written in Python using Django REST Framework.

Installing using Github
Install PostgresSQL and create db

git clone https://github.com/IvanStored/cinema-api-docker.git
cd cinema-api-docker
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=db
set DB_NAME=app
set DB_USER=MAO
set DB_PASSWORD=MAO1654
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
Run with Docker
Docker should be installed

docker-compose build
docker-compose up
Getting access
Create user : api/user/register
Get token: api/user/token
Features
JWT authenticated
Admin panel
Documentation is located at /api/doc/swagger/
Managing orders and tickets
Creating cinema halls
Creating movies with genres, actors
Adding movie sessions
Filtering movies and movie sessions
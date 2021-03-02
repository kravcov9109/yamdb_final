Workflow status badge

![yamdb_final workflow](https://github.com/kravcov9109/yamdb_final/workflows/yamdb_final%20workflow/badge.svg)

# server_name

178.154.234.96

# Continuous Integration and Continuous Deployment

Continuous Integration and Continuous Deployment YMDB_FINAL project.

## Getting Started

These instructions will allow you to set up automatic test runs, image updates on Docker Pub, and automatic deployment to the battle server when you push to the main branch.

### Prerequisites

What things you need to install the software and how to install them

asgiref==3.2.7
atomicwrites==1.4.0
attrs==19.3.0
certifi==2020.4.5.1
chardet==3.0.4
colorama==0.4.4
Django==3.0.5
django-filter==2.4.0
djangorestframework==3.11.0
djangorestframework-simplejwt==4.4.0
idna==2.9
importlib-metadata==1.6.0
more-itertools==8.2.0
packaging==20.3
pluggy==0.13.1
py==1.8.1
PyJWT==1.7.1
pyparsing==2.4.7
pytest==5.4.1
pytest-django==3.9.0
pytz==2019.3
requests==2.23.0
six==1.14.0
sqlparse==0.3.1
urllib3==1.25.9
wcwidth==0.1.9
zipp==3.1.0
gunicorn==20.0.4
psycopg2-binary==2.8.5

## Running the tests

All tests for check this project in .\yamdb_final\tests
You can use "pytest":
python manage.py pytest
or
pytest

### Steps

git clone https://github.com/kravcov9109/yamdb_final.git
All code for set up automatic test runs, image updates on Docker Pub, and automatic deployment to the battle server when you push to the main branch in .github/workflows/yamdb.yaml
Make the following changes on your Actions secrets on the GitHub:
Change your DOCKER_USERNAME, DOCKER_PASSWORD for Push Docker image to Docker Hub.
Change your HOST, USER, PASSPHRASE and SSH_KEY for executing remote ssh commands to deploy
Change your TELEGRAM_TO (telegram id) and TELEGRAM_TOKEN for message in your telegram bot.
Migrations and load data in the database:
docker-compose run web python manage.py makemigration
docker-compose run web python manage.py migrate
docker-compose run web python manage.py loaddata fixtures.json


## Authors

* **Vitaly Kravtsov** - *Yandex Praktikum* - [github.com/kravcov9109](https://github.com/kravcov9109)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Yandex Praktikum
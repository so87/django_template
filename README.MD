# Django Template

## Start developing
* You need docker installed - this should also work on windows if you have git bash installed

1. git clone https://github.com/so87/django_template.git
2. cd django_template
3. ./create-app *insert your app name here*
4. edit A_MainSite/urls.py and start-django.sh file to point to your app you just created
5. start developing - do "docker-compose up" to start up all the containers and visit "localhost:8080" to view what you create

* do "./django-shell.sh" to easily get a shell on your django machine. this is to run django commands while developing.
* mozilla has a great django tutorial

## Deploy to production
1. create gateway network "docker network create --driver overlay gateway" 
2. setup traefik to allow this to be your proxy "https://docs.traefik.io/"(this might take you a several hours to understand)
3. docker-compose -f docker-compose-production.yml


## To do 
* troubleshoot production deployment
* eliminate vulnerabilities in packages
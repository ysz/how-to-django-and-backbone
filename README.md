# how-to-django-and-backbone

## Setup

- (pip install -r requirements.txt)

- create PostgreSQL database

    $ createdb -E UTF-8 myapp

- makemigrations

    $ cd myapp
    $ python ui.py makemigrations myapp

- then apply the migrations

    $ python ui.py migrate

## How to run ui

    $ gunicorn ui --log-file=-

On OS X do

    $ echo 'backend: TkAgg' >>  ~/.matplotlib/matplotlibrc

to workaround matplotlib in virtualenv 

## How to run ONLY app.js

Get http-server

    $ sudo npm install http-server -g

and run 

    how-to-django-and-backbone/myapp $ http-server 
    
and open http://127.0.0.1:8081/home.html in Chrome dev tools





# base_drqd_project
Base project to use [Django RQ Dashboard](https://github.com/brutasse/django-rq-dashboard)

## Install

* ```git clone https://github.com/ihuro/base_drqd_project.git drqd```
* ```cd drqd```
* ```pip install -r reuirements.txt```
* ```./manage.py migrate```
* ```./manage.py createsuperuser```

## Configuration
Check https://github.com/brutasse/django-rq-dashboard if you need special settings to Redis

## Use

### Local server for testing

* ```$ ./manage.py runserver```

> Now, you can access to http://127.0.0.1:8000/admin to use it.

### Production server using gunicorn

#### Install gunicorn

[activate your virtualenv if required]

* ```pip intall gunicorn```

#### Run application

* ```gunicorn --chdir [path_to_drqd_folder] -w 2 -b 0.0.0.0:8000 dashboard.wsgi:application```

> Now, you can access to http://your_server:8000/admin to use it.

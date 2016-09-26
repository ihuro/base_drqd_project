# base_drqd_project
Base project to use Django RQ Dashboard

## Install
git clone https://github.com/ihuro/base_drqd_project.git drqd
cd drqd
pip install -r reuirements.txt
./manage.py migrate
./manage.py createsuperuser

## Configuration
Check https://github.com/brutasse/django-rq-dashboard if you need special settings to Redis

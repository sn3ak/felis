# felis
django-based web-application to manage FreeBSD jails

Working on Documenting this project.

Installation Instructions

Download Code

Install requirements with pip -r requirements.txt (to be posted soon)

Edit settings.py in the felis directory 

 Create a secure SECRET_KEY
 
 Add your Hosts to ALLOWED_HOSTS
 
 Change DATABASES settings to match your environment
 
 Setup redis database and update CACHES to match your environment
 
 Change FELIS_WORK_DIR to match your environment
 
Run ./manage.py migrate felis to create the inital DB

Run ./manage.py migrate selfcheck to add it's support to the DB

Run ./manage.py createsuperuser to create your initial user

Run ./manage.py runserver to start the application

Run ./manage.py qcluster for running scheduled tasks

Connect to the web interface by browing to IP:8000 


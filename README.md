# felis
a fork of [vonabarak/felis](https://github.com/vonabarak/felis).

A django-based web-application to manage FreeBSD jails.

Working on Documenting this project.

# Table of Contents
- [felis](#felis)
- [Package Requirements](#package-requirements)
- [felis Installation](#felis-installation)
  
# Package Requirements
## Install the following packages on the jail host
1. `pkg install postgresql13-client sudo sqlite3 python39 py39-pip py39-sqlite3 py39-supervisor py39-virtualenv`
   
# felis Installation
## Setup a virtual environment

## felis Installation
1. Download Code
2. `pip -r requirements.txt`
3. edit felis/settings.py
    * Create a secure SECRET_KEY
    * Add host IP to ALLOWED_HOSTS
    * Change DATABASE settings
    * Update CACHES
    * Update Q_CLUSTER
    * Change FELIS_WORK_DIR
4. `manage.py migrate felis` Create initial Database
5. `manage.py migrate selfcheck` - May not be needed. Need to update notes
6. `manage.py createsuperuser` to create your initial user
7. `manage.py runserver 0.0.0.0:8000` Start application
8. `manage.py qcluster` Start Scheduled tasks application

## Web Interface
Connect to the web interface by at Host_IP:8000 

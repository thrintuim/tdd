Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3.6
* virtualenv + pip
* Git

eg, on Ubuntu:
	
	sudo apt update
	sudo apt-get install nginx git python3.6 python3.6-venv

## Nginx Virtual Host confix

* see nginx.template.conf
* replace DOMAIN with, e.g., staging.my-domain.com

## Systemd service

* see gunicorn-systemd.template.service
* replace DOMAIN with, e.g., staging.my-domain.com

## Folder structure:

/home/username
|--sites
  |--DOMAIN1
  |  |-- .env
  |  |-- db.sqlite3
  |  |-- manage.py etc
  |  |-- static
  |  |-- virtualenv
  |--DOMAIN2
     |-- .env
     |-- db.sqlite3
     |-- etc 

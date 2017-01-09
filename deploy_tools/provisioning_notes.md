Provisioning a new site
=======================

## Required packages 

* nginx
* Python 3
* Git
* pip
* virtualenv

e.g., on Ubuntu:

	sudo apt-get install nginx git python3 python3-pip
	sudo pip3 install virtualenv

## nginx Virtual Host config

* See nginx.template.conf
* replace SITENAME with, e.g. staging.my-domain.com

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, e.g. staging.my-domain.com

## Folder Structure
Assume we have a user account at /home/username

/home/username
	sites
		SITENAME
			database
			source
			static
			virtualenv
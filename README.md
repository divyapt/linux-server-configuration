# Linux Server Configuration

## IP Address
54.214.170.163

## URL
http://54.214.170.163:80
Above is the URL that is supposed to be accessed, but App is still not working because of the following error:
I am hoping to get some help with this from the reviewer, since i have tried a lot of things

[Thu Apr 11 09:03:29.481556 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] mod_wsgi (pid=20366): Target WSGI script '/var/www/catalog/catalog.wsgi' cannot be loaded as Python module. [Thu Apr 11 09:03:29.481728 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] mod_wsgi (pid=20366): Exception occurred processing WSGI script '/var/www/catalog/catalog.wsgi'. [Thu Apr 11 09:03:29.482014 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] Traceback (most recent call last): [Thu Apr 11 09:03:29.482119 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] File "/var/www/catalog/catalog.wsgi", line 8, in <module> [Thu Apr 11 09:03:29.482198 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] from catalog import app as application [Thu Apr 11 09:03:29.482293 2019] [wsgi:error] [pid 20366:tid 139818966742784] [remote 70.95.200.202:0] ImportError: cannot import name 'app' [Thu Apr 11 09:03:29.583587 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] mod_wsgi (pid=20366): Target WSGI script '/var/www/catalog/catalog.wsgi' cannot be loaded as Python module. [Thu Apr 11 09:03:29.583781 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] mod_wsgi (pid=20366): Exception occurred processing WSGI script '/var/www/catalog/catalog.wsgi'. [Thu Apr 11 09:03:29.583949 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] Traceback (most recent call last): [Thu Apr 11 09:03:29.584088 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] File "/var/www/catalog/catalog.wsgi", line 8, in <module> [Thu Apr 11 09:03:29.584168 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] from catalog import app as application [Thu Apr 11 09:03:29.584277 2019] [wsgi:error] [pid 20366:tid 139819050743552] [remote 70.95.200.202:21281] ImportError: cannot import name 'app'

## Summary of software Installed
* Postgres
* Apache2
* Flask
* SQAlchemy
* Requests
* Oauth2Client

## Summary of configurations made
* Add user grader, Give sudo access to "grader" user.
* Configuring key based authentication to the "grader" user.
* Enforcing Key-based SSH authentication  .
* Configure Firewall to enable SSH, HTTP and NTP 
* Install tomcat and ensure webserver is running on port 80
* Configure web server to serve the Item Catalog application - yet to be completed , stuck with error.

## List of third-party resources
* https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps


## Authors
* **Divya Tuduma**
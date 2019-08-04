# Linux-Server-Config
Took a baseline installation of linux distribution on a virtual machine and prepared it to host Item Catalog web application. Installed/updated required packages, configured web and database servers and secured it from a number of attack vectors.

* EC2 URL : http://ec2-13-233-0-120.ap-south-1.compute.amazonaws.com 
* IP Address : http://13.233.0.120.xip.io
* SSH Port : 2200

## Softwares/Packages installed
* Flask
* httplib2
* psycopg2
* oauth2client
* requests
* Sqlalchemy
* apache2
* libapache2-mod-wsgi

## Configurations done
* Created a user named 'grader'. Gave sudo permissions to it.
* Changed the ssh port from 22 to 2200.
* Generated a ssh keypair and used it for login. Removed root login without password.
* Configured the local timezone to UTC.
* Configured the UFW Firewall to allow ssh(2200), http(80) and ntp(123) ports.
* Configured apache to serve python mod_wsgi application.
* Clone the git repository to the server.
* Installed postgresql for database and for oauth2 login modified redirect_uris and supported javascript domains.

## Resources
* https://medium.com/@rodkey/deploying-a-flask-application-on-aws-a72daba6bb80
* https://medium.com/@dushan14/create-a-web-application-with-python-flask-postgresql-and-deploy-on-heroku-243d548335cc
* https://docs.sqlalchemy.org/en/13/dialects/postgresql.html
* https://hackernoon.com/flask-web-programming-from-scratch-9ada8088fde1






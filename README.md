# Udacity-Linux-Server
Final project for FSND - Linux server configuration

## Accessing the application on Amazon Lightsail
- The website can be accessed at http://ec2-52-34-116-134.us-west-2.compute.amazonaws.com/ (IP address is 52.34.116.134)
- SSH is set up on port 2200. 
- The public key for the grader account has already been set up on the server. The private key will be supplied on submission. 
- The grader account has sudo access and does not require a password to do so.

## Software installed on Ubuntu
emacs, postgresql, postgresql-contrib, apache2, libapache2-mod-wsgi, python-pip

## Python packages installed
Flask, sqlalchemy, httplib2, oauth2client, requests, psycopg2

## Configuration changes made to the existing application
- Changed the DB connection string from using sqlite to postgresql in application.py, setup.py and populate.py
- added an empty __init__.py file that is required for Python 2.x WSGI applications
- Fixed a couple of small, unrelated-to-this-project bugs in the application

## Resources
I read the following articles in order to learn how to secure a Linux server and make the application work on Apache with WSGI.
- https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-16-04
- http://cubicspot.blogspot.com/2017/05/secure-web-server-permissions-that-just.html
- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
- https://discussions.udacity.com/t/problems-with-the-digital-ocean-tutorial/336376
- https://www.theodo.fr/blog/2017/03/developping-a-flask-web-app-with-a-postresql-database-making-all-the-possible-errors/

# Linux-Server-Configuration Udacity
Done using Digital Ocean 
- Ip address is :45.55.47.62
- URL to the server : http://45.55.47.62/
# Steps To log in
- open terminal
- Run Vagrant up and vagrant ssh
- key in `ssh grader@45.55.47.62 -p 2200`
- type the password for the grader and now logged into the digital ocean server.
# Summary
- Add a new user grader using `sudo adduser grader`
- Give grader sudo permission
- Set-up Key-based Authentication/Public Key Encryption using ssh-keygen
- Added Public Key to Server using `mkdir .ssh` `touch .ssh/authorized_keys`
-  Disabled Password Based Login and Force Login using Key Pair
- Update all currently installed packages using `sudo apt-get update`
- Change the SSH port from 22 to 2200
- Configure Firewall to only allow incoming connections for SSH (port 2200),
- Install and configure Apache to serve a Python mod_wsgi application
- Install and configure PostgreSQL
- Created wsgi file as per documentation
- Install App dependencies for Flask and Database
```
sudo pip install Flask
sudo pip install sqlalchemy
sudo pip install Flask-SQLAlchemy
sudo pip install psycopg2
sudo apt-get install python-psycopg2 
sudo pip install flask-seasurf
sudo pip install oauth2client
sudo pip install httplib2
sudo pip install requests
```
- Modified Engine to serve the database

# Refrences
- Reference Documentation: https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-12-04 
https://wiki.knownhost.com/security/misc/how-can-i-change-my-ssh-port
- Reference documentation: https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps 
https://help.ubuntu.com/community/PostgreSQL 
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04
- Reference Documentation: https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps
- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps



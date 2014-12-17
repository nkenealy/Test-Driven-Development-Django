## Required packages:

* nginx
* Python 3
* Git
* pip
* virtualenv

eg on ubuntu:

   sudo apt-get install nginx git python3 python3-pip
   sudo pip3 install virtualenv

   ## Nginx Virtual Host config

   * se nginx.template.conf
   * replace SITENAME with, eg, staging.my-domain.com

   ## Upstart Job
   see gunicorn-upstart,template.conf
   * replace SITENAME with ,eg, staging.my-domain.com

   ## FOlder structure

   Assume we have a user account at /home/username

   /home/username
       sites
           SITENAME
                 database
                 source
                 static
                 virtualenv


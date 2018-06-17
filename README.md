# Linux Server Configuration

Fresh Ubuntu VPS by Amazon Lightsail. This is used to host my [Item Catalog application](https://github.com/myasul/catalog).

### Summary of Changes
* Installed applications using apt-get is saved in software_installed_list.txt.
* Installed libraries using pip is saved in python_libraries_installed_list.txt.
* Created a user <grader> which has sudo access.
* The server can only be accessed using SSH keys.
* The server is firewall-enabled and only accepts incoming requests from port 80, 2200 and 143.
* The server can only be remotely accessed via port 2200.
* Item Catalog application is deployed using Apache/2.4.18 (Ubuntu).
* Web server has been configured to serve the Item Catalog application as a WSGI app.
* Persistent data are saved in PostgreSQL 9.5.13.
* All system packages are up-to-date.
* Used static IP address <35.180.72.153>.
  
### Website Details
* URL: http://www.35.180.72.153.nip.io/

### Third Party Sources
* Used [nip.io](http://nip.io/) to be able to use Google's OAuth feature.
* Used [Amazon Lightsail](https://aws.amazon.com/lightsail/) to be able to create my own Ubuntu VPS.
  
### Guides used
* [How To Deploy a Flask Application on an Ubuntu VPS](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps) by Kundan Singh
* [LAMP Stack, Python Flask, PostgreSQL and Apache Mod_WSGI on Ubuntu 16.04](https://www.topikettunen.com/2018/02/01/h3-linux-palvelimet-ict4tn021-8.html) by Topi Kettunen
* [Deploy Flask & Python3 on Apache2 & Ubuntu](http://terokarvinen.com/2016/deploy-flask-python3-on-apache2-ubuntu) by Tero Karvinen

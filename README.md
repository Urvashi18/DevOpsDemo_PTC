# DevOpsDemo_PTC
Description :
This ansible script will 
1. Setup
 - Apache httpd
 - tomcat
 - mod_jk
 - mysql 

2. Configure
  - To start two tomcat instances
  - mod_jk 
  - enable proxy
  - restart apache2 and tomcat7

Script deploy the petstore project which will be used to test the above setup.
Mention host name in hosts file, can configure any number of hosts
Mention port numbers where tomcat instances will run in conf.yml

Run the script with following command :
ansible-playbook --user ubuntu --ask-pass --ask-become-pass -i hosts site.yml
and
Provide ssh passsword and the sudo password
After the script runs successfully.

Open the browser and use following url:
http://<hostname>/petstore

e.g. http://23.20.175.66/petstore/
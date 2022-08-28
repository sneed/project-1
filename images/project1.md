## Project1 Documentation

### STEP 1 — INSTALLING APACHE AND UPDATING THE FIREWALL
`sudo apt update`
![Package Information](../images/package-info.png)

`sudo apt install apache2`
![Apache2 package installation](../images/apache-installation.png)

`sudo systemctl status apache2`
![Apache running as a service on Ubuntu](../images/apache-asaservice.png)

`curl http://localhost:80`
![Apache Server on port 80](../images/apache-onubuntushell.png)

![Web server installed](../images/webserver-installed.png)

### STEP 2 — INSTALLING MYSQL

`sudo apt install mysql-server`
![Acquire and Install mysql-server ](../images/mysql-server.png)

`sudo mysql`
![Log into mysql-server console](../images/mysql-server-console.png)

### STEP 3 — INSTALLING PHP

`sudo apt install php libapache2-mod-php php-mysql
php -v`
![Php package and Module](../images/php-packages.png)

### STEP 4 — CREATING A VIRTUAL HOST FOR YOUR WEBSITE USING APACHE

`sudo mkdir /var/www/projectlamp`
![Create the directory for 'projectLamp' using ‘mkdir’ command](../images/makedir-projectlamp.png)

`sudo nano /etc/apache2/sites-available/projectlamp.conf`
![configuration file in Apache’s sites-available directory](../images/apache-configfile.png)

`sudo ls /etc/apache2/sites-available`
![List the new file in the sites-available directory](../images/sites-available.png)


### STEP 5 — ENABLE PHP ON THE WEBSITE

`sudo nano /etc/apache2/mods-enabled/dir.conf`
![Default DirectoryIndex settings on Apache](../images/apachedir-config.png)

`nano /var/www/projectlamp/index.php`
![Create php file inside custom web root folder](../images/project1.md)
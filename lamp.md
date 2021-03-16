# DEPLOYING A LAMP STACK
First, I installed Ubuntu on a virtualbox then i took these steps;

*Step 1 — Installing Apache and Updating the Firewall*

I installed Apache using Ubuntu’s package manager *apt*


`$ sudo apt update`

`$ sudo apt install apache2`

![package upgrade](https://github.com/olateekay/deploying-lamp-stack/blob/main/images/lamp1.JPG)

![apache install](https://github.com/olateekay/deploying-lamp-stack/blob/main/images/lamp2.JPG)

`$ sudo systemctl status apache2`

![apache status](images\lamp3.jpg)

I enabled the firewall on the server

`sudo ufw enable`

`sudo ufw allow "Apache"`

![apache status](images\lamp4.jpg)


![apache status](images\lamp5.jpg)

check how if you can access it locally in the Ubuntu shell by running,

`curl http://localhost:80`

![apache status](images\lamp6.jpg)

open a web browser and try to access the url,

`http://<Public-IP-Address>:80`

![apache status](images\lamp7.jpg)


*Step 2 — Installing MySQL*

`$ sudo apt install mysql-server`

![apache status](images\lamp8.jpg)

Run this script to remove some insecure default settings and lock down access to the database system.

`$ sudo mysql_secure_installation`

![apache status](images\lamp9.jpg)

Test if you’re able to log in to the MySQL console by typing;

`$ sudo mysql`

![apache status](images\lamp10.jpg)


*Step 3 — Installing PHP*

 PHP is the component of our setup that will process code to display dynamic content to the end user. In addition to the php package, you’ll need php-mysql, a PHP module that allows PHP to communicate with MySQL-based databases. You’ll also need libapache2-mod-php to enable Apache to handle PHP files.

 To install these 3 packages at once, run:

 `$ sudo apt install php libapache2-mod-php php-mysql`

![apache status](images\lamp11.jpg)

 Once the installation is finished, you can run the following command to confirm your PHP version:

 `php -v`

 ![apache status](images\lamp12.jpg)







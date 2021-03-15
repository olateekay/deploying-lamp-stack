# DEPLOYING A LAMP STACK
First, I installed Ubuntu on a virtualbox then i took these steps;

*Step 1 — Installing Apache and Updating the Firewall*

I installed Apache using Ubuntu’s package manager *apt*


`$ sudo apt update`

`$ sudo apt install apache2`

![package upgrade](images\lamp1.jpg)

![apache install](images\lamp2.jpg)

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







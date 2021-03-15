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







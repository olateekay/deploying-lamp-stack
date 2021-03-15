# DEPLOYING A LAMP STACK
First, I spinned up an EC2 instance with Ubuntu Server OS. Then i took these steps;

*Step 1 — Installing Apache and Updating the Firewall*

I installed Apache using Ubuntu’s package manager *apt*


`$ sudo apt update`

`$ sudo apt install apache2`

![package upgrade](images\lamp1.jpg)

![apache install](images\lamp2.jpg)

`$ sudo systemctl status apache2`

![apache status](images\lamp3.jpg)



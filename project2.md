# **PROJECT 2: LEMP STACK IMPLEMENTATION**

___
### **TASK 1: INSTALLING THE NGINX WEB SERVER**
___

I ran the following commands on my virtual machine to update a list of packages in the Ubuntu package manager, to install ngnix and to verify that it is running as a service in my OS:


`sudo apt update`

`sudo apt install ngnix`

`sudo systemctl status ngnix`

The outcome is depicted in the image below:
![Nginx Status](./images/active_nginx.PNG 'Nginx Status')

A new rule was then added to the EC2 configuration to open inbound connection through port 80, shown below:

![Inbound Connection Permitted](./images/Inbound-connection-permitted.PNG 'Inbound Connection Permitted')


Next, I checked that my Nginx server can be accessed locally in my virtual machine. The result is displayed below:

![Nginx Server in Ubuntu](./images/nginx-in-ubuntu.PNG "Nginx Server in Ubuntu")


---
### **TASK 2: INSTALLING MYSQL**
___

MySQL software was installed on my OS by running the following command:

`sudo apt install mysql-server`

The outcome is shown below

![MySQL Installation](./images/mysql-installation.PNG 'MySQL Installation')

This step was immediately followed by running the secruity script. This was done with the command below, to which I responded with any other key besides 'Y':

`sudo mysql_secure_installation`

This step was immediately followed by running the secruity script. This was done with the command below, to which I responded with any other key besides 'Y':

`sudo mysql_secure_installation`

Thereafter, I logged in to the MySQL console by running this command:

`sudo mysql`

The outcome is shown below:

![MySQL Console](./images/mysql-console.PNG 'MySQL Console')
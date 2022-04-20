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
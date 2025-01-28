# Azure Networking Project: Nginx on Virtual Machine with Firewall

##  Overview
This project demonstrates setting up a **secure web server on Azure** using **Azure Virtual Network (VNet), Virtual Machine (VM), Azure Firewall, and Bastion**.

##  Technologies Used
- Azure Virtual Network (VNet), Virtual Machine (VM)
- Azure Firewall, Azure Bastion, DNAT Rules
- Nginx Web Server (on Ubuntu)
- Linux commands for configuration

##  Steps Involved
Created a Virtual Network (VNet) with a subnet.

-Deployed a Virtual Machine (VM) inside the subnet.

-Installed & Configured Nginx on the VM by using to serve a static HTML page.

- Set Up Azure Bastion for secure, browser-based access to the VM (without exposing SSH/RDP).

- Configured Azure Firewall to protect the network and control traffic.

- Implemented DNAT Rules to forward HTTP requests to the VM securely.

-Tested & Successfully Accessed the Web Server via the Firewall’s public IP.

##  Linux Commands Used
```bash
sudo apt update && sudo apt install nginx -y
sudo systemctl start nginx
sudo nano /var/www/html/index.html
curl localhost:80

##  Accessing the Web Page
Visit http://20.231.67.26:80

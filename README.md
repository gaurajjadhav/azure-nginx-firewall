# Azure Networking Project: Nginx on Virtual Machine with Firewall

##  Overview
This project demonstrates setting up a **secure web server on Azure** using **Azure Virtual Network (VNet), Virtual Machine (VM), Azure Firewall, and Bastion**.

##  Technologies Used:
- Azure Virtual Network (VNet), Virtual Machine (VM)
- Azure Firewall, Azure Bastion, DNAT Rules
- Nginx Web Server (on Ubuntu)
- Linux commands for configuration

##  Steps Involved:
1. Created a Virtual Network (VNet) with a subnet.

2. Deployed a Virtual Machine (VM) inside the subnet.

3. Installed & Configured Nginx on the VM by using to serve a static HTML page.

4. Set Up Azure Bastion for secure, browser-based access to the VM (without exposing SSH/RDP).

5. Configured Azure Firewall to protect the network and control traffic.

6. Implemented DNAT Rules to forward HTTP requests to the VM securely.

7. Tested & Successfully Accessed the Web Server via the Firewall’s public IP.

##  Linux Commands Used
```bash
sudo apt update && sudo apt install nginx -y
sudo systemctl start nginx
sudo nano /var/www/html/index.html
curl localhost:80


📡 Accessing the Web Page
Visit http://20.231.67.26:4000


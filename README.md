# Azure Networking Project: Nginx on Virtual Machine with Firewall

##  Overview
This project demonstrates setting up a **secure web server on Azure** using **Azure Virtual Network (VNet), Virtual Machine (VM), Azure Firewall, and Bastion**.

##  Technologies Used
- Azure Virtual Network (VNet), Virtual Machine (VM)
- Azure Firewall, Azure Bastion, DNAT Rules
- Nginx Web Server (on Ubuntu)
- Linux commands for configuration

##  Steps Involved
1. Created a Virtual Network and Subnet.
2. Deployed a Virtual Machine and installed Nginx.
3. Configured Azure Firewall and DNAT rules.
4. Set up Bastion for secure access.
5. Hosted a static HTML page on Nginx.

##  Linux Commands Used
```bash
sudo apt update && sudo apt install nginx -y
sudo systemctl start nginx
sudo nano /var/www/html/index.html
curl localhost:80

Accessing the Web Page
Visit http://20.231.67.26:80

# Azure Networking Project: Nginx on Virtual Machine with Firewall

##  Overview
This project built and configured to a secure web server on Microsoft Azure using key networking and security components. This project focused on setting up a Virtual Machine (VM) with Nginx, managing network access using Azure Firewall and Bastion, and implementing DNAT rules for external access.

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

## Linux Commands Used:
During the setup and configuration, I used the following Linux commands:

🔹 Updating and Installing Nginx:
sudo apt update
sudo apt install nginx -y

🔹 Checking Nginx Status:
sudo systemctl status nginx

🔹 Restarting Nginx After Configuration Changes:
sudo systemctl restart nginx

🔹 Editing the Default HTML Page:
sudo nano /var/www/html/index.html

🔹 Testing the Web Server Locally:
curl localhost:80

🔹 Checking If Port 80 Is Open:
sudo netstat -tulnp | grep :80

🔹 Verifying Nginx Configuration:
sudo nginx -t

## Project Outcome:
This project strengthened my hands-on experience with Azure networking, security, and cloud infrastructure while enhancing my knowledge of Linux commands for server management.

## 📡 Accessing the Web Page
Visit http://20.231.67.26:4000


# Secure-Web-Hosting-with-Firewall-and-NGINX-on-Azure
This project demonstrates how to securely host a web application on Microsoft Azure using NGINX within a Virtual Machine (VM), protected by an Azure Firewall. It ensures secure access while regulating inbound and outbound traffic to enhance security.

# Overview

This project demonstrates how to securely host a web application on Microsoft Azure using NGINX within a Virtual Machine (VM), protected by an Azure Firewall. It ensures secure access while regulating inbound and outbound traffic to enhance security.

# Achitecture

The project follows this architecture:<br><br>
Azure Virtual Network (VNet): Configured to create a secure network environment.<br>
Azure Subnet: A dedicated subnet within the VNet to host the virtual machine and firewall.<br>
Azure Firewall: Configured to regulate traffic, allowing only specific requests to reach the VM.<br>
Azure Virtual Machine (VM): Deployed to host the web application using NGINX.<br>
NGINX Web Server: Installed on the VM to serve an HTML page securely.

# Features
Secure VNet and Subnet: Ensures controlled communication within Azure resources.

Azure Firewall Protection: Regulates access to the VM, preventing unauthorized access.

NGINX Web Hosting: Provides a lightweight and efficient web server.

Controlled Traffic Routing: Ensures that users can securely access content while bypassing unauthorized requests.

# Prerequisites

Before deploying this solution, ensure you have:

An active Azure account

Azure CLI installed (Installation Guide)

Basic knowledge of Azure networking and Linux commands

# Deployment Steps

1. Create a Virtual Network (VNet)<br>
  <h4>az network vnet create --resource-group MyResourceGroup --name MyVNet --address-prefix 10.0.0.0/16</h4>

2. Create a Subnet
<h4>az network vnet subnet create --resource-group MyResourceGroup --vnet-name MyVNet --name MySubnet --address-prefix 10.0.1.0/24</h4>
   

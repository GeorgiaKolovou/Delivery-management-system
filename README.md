# Delivery-management-system

# GreenGrocer Delivery Management System

This project presents the transformation of a local business called GreenGrocer into an online store through the implementation of a client-server infrastructure.
The system was developed using a virtual machine environment and includes a web server, database server, and automation scripts for system maintenance.
This project was developed as part of the Computing Infrastructure module in the BSc (Hons) Computing programme.

---

## System Overview

The purpose of this project is to design a simple infrastructure that supports online ordering and delivery management for a local business.
The system includes:

- A web server hosting a WordPress website
- A MariaDB database to manage business data
- A virtual machine running Linux
- Automation scripts for system maintenance and monitoring

The infrastructure allows the business to manage customer orders and delivery operations through an online platform.  

---

## Virtual Machine Infrastructure

The system is deployed on a virtual machine created using VirtualBox with Linux Mint.
The virtual machine was configured with:

- 4 GB RAM
- 1 CPU core
- 100 GB storage

These resources ensure that the server can support the workload of the delivery management system.  

---

## Server Configuration

The server environment includes the following components:

- **Apache2** – Web server hosting the website
- **MariaDB** – Database management system
- **PHP** – Processing dynamic web content

Together, these technologies create a typical LAMP-style infrastructure that allows the system to store data and serve dynamic web pages.  

---

## Website Implementation

The website was created using WordPress, which allows easy management of the online store.
Additional plugins were used to support delivery management:

- WooCommerce
- Delivery & Pickup Date Time for WooCommerce
- Local Delivery Drivers for WooCommerce

These plugins allow the system to manage orders, assign drivers and select delivery times.  

---

## Automation Scripts

The system includes several automation scripts to improve reliability and reduce manual work.

### Backup Script
The backup script creates daily backups of:

- the WordPress website files
- the MariaDB database

The script also produces a log file showing when each backup was executed.

### Monitoring Script
The monitoring script checks:

- CPU usage
- Memory usage

If usage exceeds predefined limits, the script records an alert in a log file.

### Update Script
The update script automatically updates the system packages during off-peak hours to ensure system stability and security.  

---

## Cron Automation

All automation scripts are scheduled using cron jobs:

- Backup script → runs daily at 1:00 AM
- Monitoring script → runs twice daily at 9:00 AM and 9:00 PM
- Update script → runs daily at 6:00 AM

Cron allows the system to perform maintenance tasks automatically without manual intervention.  

---

## System Testing

The system was tested by accessing the web server through the virtual machine’s IP address and port configuration.
Through the WordPress dashboard, the administrator can:

- manage customer orders
- assign drivers
- configure delivery times

This confirms that the infrastructure and web server are functioning correctly.  

---

## Future Improvements

Future improvements for the system could include:

- additional automation scripts
- enhanced security and encryption
- improved user interface for customers
- postcode-based delivery availability checking

These improvements would make the system more secure and scalable for real-world deployment. 

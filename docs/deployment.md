# PrestaShop Deployment Guide

## 1. Project Objective
Deploy PrestaShop on AWS using two separate Ubuntu EC2 instances: one for the application and one for the database.

## 2. Application Server Setup
- Launched an Ubuntu EC2 instance for the application.
- Installed and configured Apache HTTP Server.
- Installed PHP and the required application extensions.
- Deployed PrestaShop files.
- Configured the application to communicate with the database server.

## 3. Database Server Setup
- Launched a separate Ubuntu EC2 instance for the database.
- Installed and configured MariaDB.
- Created the PrestaShop database and configured database connectivity.
- Configured MariaDB to listen on the database server's private network address.

## 4. Network Configuration
- Configured AWS security groups to control inbound traffic.
- Allowed web traffic to the application server.
- Restricted database traffic on TCP port 3306 to the application server's security group.
- Used the database server's private IP address for application-to-database communication.
- Kept the database server without a public IP address.

## 5. Validation and Troubleshooting
- Checked EC2 instance status and connectivity.
- Troubleshot package installation and network connectivity issues.
- Verified that the application server could connect to MariaDB.
- Confirmed that PrestaShop's web interface loaded successfully.

## 6. Security Considerations
- The demonstration uses HTTP; configure HTTPS before production use.
- Restrict SSH access to trusted sources.
- Never publish private keys, passwords, database credentials, or AWS access keys.
- Apply security updates and configure backups and monitoring.

## 7. Outcome
Successfully deployed the PrestaShop web application with a separate MariaDB database server, demonstrating hands-on cloud deployment, Linux administration, network troubleshooting, and basic infrastructure security.
Successfully deployed the PrestaShop web application with a separate MariaDB database server, demonstrating hands-on cloud deployment, Linux administration, network troubleshooting, and basic infrastructure security.


# AWS PrestaShop Deployment with Separate Application and Database Servers

## Project Overview
Deployed a PrestaShop e-commerce application on AWS using a two-server architecture, separating the application server from the database server.

This project demonstrates practical experience with cloud infrastructure, Linux administration, database connectivity, network security, and web application deployment.

## Architecture
- **Application server:** Ubuntu EC2 instance running Apache, PHP, and PrestaShop.
- **Database server:** Separate Ubuntu EC2 instance running MariaDB.
- **Database connectivity:** Private communication between the application and database servers.
- **Web access:** HTTP access to the application through the application server's public IP.
- **Cloud platform:** Amazon Web Services (AWS).

## Security Measures
- Separated the application and database workloads across two servers.
- Restricted database access to the application server's security group on TCP port 3306.
- Configured database connectivity using the database server's private IP address.
- Kept the database server without a public IP address.
- Configured network access through AWS security groups.

## Technologies Used
- Amazon EC2
- AWS VPC and Security Groups
- Ubuntu Linux
- Apache HTTP Server
- PHP
- MariaDB
- PrestaShop
- Linux command-line administration

## Skills Demonstrated
- Cloud infrastructure deployment
- Linux server administration
- Network troubleshooting
- Database configuration and connectivity
- Security group configuration
- Multi-tier application architecture
- Web application deployment and troubleshooting

## Lessons Learned
This project provided hands-on experience troubleshooting server connectivity, configuring database access, resolving package installation issues, and deploying an application across separate cloud instances.

## Disclaimer 
This project was created for educational and portfolio purposes. Production deployments require HTTPS, secure secrets management, regular patching, backups, monitoring, and additional hardening.
This project was created for educational and portfolio purposes. Production deployments require HTTPS, secure secrets management, regular patching, backups, monitoring, and additional hardening.

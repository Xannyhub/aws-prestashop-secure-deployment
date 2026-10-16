# AWS PrestaShop Architecture

## Overview
This project deploys a PrestaShop e-commerce application on AWS using a separate application server and database server.

## Infrastructure Components

### 1. Application Server
- Operating system: Ubuntu Linux
- Web server: Apache HTTP Server
- Application runtime: PHP
- Application: PrestaShop
- Role: Receives HTTP requests and serves the web application.

### 2. Database Server
- Operating system: Ubuntu Linux
- Database engine: MariaDB
- Role: Stores PrestaShop application data.
- Network configuration: No public IP address; accessed through private networking.

## Network and Security Design
- The application server is publicly accessible over HTTP for the deployment demonstration.
- The database server communicates with the application server over its private IP address.
- The database security group restricts TCP port 3306 to the application server's security group.
- AWS security groups control access between the infrastructure components.

## Request Flow
1. A visitor connects to the application server.
2. Apache and PHP process the web request.
3. PrestaShop communicates with MariaDB over the private network.
4. The database returns the requested data to the application.

## Security Improvements for Production
- Configure HTTPS using TLS.
- Restrict administrative access and SSH sources.
- Keep software and operating systems patched.
- Configure database backups and recovery procedures.
- Enable centralized logging, monitoring, and alerting.
- Use secure secret management and least-privilege access controls.

## Scope

This is an educational cloud deployment project intended to demonstrate practical skills in AWS infrastructure, Linux administration, network security, database configuration, and web application deployment.

## Scope
This is an educational cloud deployment project intended to demonstrate practical skills in AWS infrastructure, Linux administration, network security, database configuration, and web application deployment.

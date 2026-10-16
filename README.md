# AWS PrestaShop Deployment — Two-Tier Architecture

## Project Overview

A hands-on cloud deployment project using Amazon Web Services (AWS), with PrestaShop hosted on a dedicated application server and MariaDB hosted on a separate database server.

The project demonstrates practical skills in cloud infrastructure, Linux administration, network security, database connectivity, and troubleshooting.

## Architecture

| Component | Implementation |
|---|---|
| Cloud platform | AWS |
| Compute | Amazon EC2 |
| Operating system | Ubuntu Linux |
| Web server | Apache HTTP Server |
| Application runtime | PHP |
| E-commerce application | PrestaShop |
| Database | MariaDB |
| Network security | AWS Security Groups |

## Architecture Diagram

See the [Architecture Diagram](docs/architecture-diagram.md) for the application and database request flow.

## Security Highlights

- Separated application and database servers.
- Configured private database connectivity.
- Restricted database access using AWS security groups.
- Kept the database server without a public IP address.

## Project Documentation

- [Architecture Overview](docs/architecture.md)
- [Deployment Guide](docs/deployment.md)
- [Security Configuration](docs/security.md)
- [Architecture Diagram](docs/architecture-diagram.md)

## Screenshots

- [EC2 Instances](screenshots/ec2-instances.png)
- [AWS Security Group Configuration](screenshots/aws-security-group.png)
- [PrestaShop Deployment](screenshots/prestashop-homepage.png)

## Skills Demonstrated

AWS EC2 · AWS Security Groups · Ubuntu Linux · Apache · PHP · MariaDB · Network Troubleshooting · Web Application Deployment

## Future Improvements

- Configure HTTPS/TLS.
- Strengthen SSH and administrative access controls.
- Implement backups, centralized logging, and monitoring.
- Review IAM permissions and server hardening.

## Disclaimer
Educational portfolio project. This deployment should not be considered production-ready without further security hardening. No credentials, private keys, or secrets should be stored in this repository.
Educational portfolio project. This deployment should not be considered production-ready without further security hardening. No credentials, private keys, or secrets should be stored in this repository.

# AWS Security Configuration

## 1. Security Objectives
The objective is to reduce unnecessary network exposure and separate the web application from the database layer.

## 2. Network Access Controls

### Application Server
- Exposes HTTP on TCP port 80 for the deployment demonstration.
- SSH access should be restricted to a trusted administrative IP address.
- Only necessary inbound ports should be permitted.

### Database Server
- Has no public IP address.
- Accepts MariaDB traffic on TCP port 3306 only from the application server's security group.
- Does not require direct public access for normal application database communication.

## 3. Security Group Design
AWS security groups act as virtual firewalls controlling inbound and outbound traffic.

The database security group uses a security-group reference to limit database connections to the designated application server security group, rather than allowing connections from every public IP address.

## 4. Security Validation
Validation performed during deployment included:
- Checking application-to-database connectivity.
- Troubleshooting network connection failures.
- Verifying MariaDB access from the application environment.
- Confirming that the web application loaded.

## 5. Recommended Hardening
- Configure HTTPS using TLS.
- Disable unnecessary services and ports.
- Use least-privilege IAM permissions.
- Protect secrets using an appropriate secrets-management solution.
- Apply operating system and application security updates.
- Enable logging, monitoring, and security alerts.
- Establish database backups and test recovery.
- Review outbound network access and administrative access regularly.

## 6. Limitations
This project is a learning environment, not a production security certification. The security controls should be reviewed and tested before the system handles real customer data.
This project is a learning environment, not a production security certification. The security controls should be reviewed and tested before the system handles real customer data.


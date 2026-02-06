# Network Enumeration Checklist

## Initial Discovery
- Identify live hosts in the target network
- Determine network range and segmentation
- Detect firewalls, gateways, and routing behavior

## Port and Service Enumeration
- Identify open TCP and UDP ports
- Enumerate running services and versions
- Detect uncommon or misconfigured services

## Protocol Enumeration
- Enumerate SMB, FTP, SSH, HTTP, DNS, SNMP where applicable
- Identify anonymous or weak access configurations
- Review banner information for potential misconfigurations

## Authentication and Access
- Identify authentication mechanisms in use
- Detect weak or default credentials exposure
- Review access control boundaries between services

## System and Infrastructure Analysis
- Identify operating systems and architectures
- Detect virtualization or containerized environments
- Map trust relationships between systems

## Findings Documentation
- Record discovered services and access points
- Identify potential attack paths
- Prepare enumeration data for exploitation phase

## Common Ports Reference

| Port | Service | Description |
|------|--------|-------------|
| 21   | FTP    | File Transfer Protocol, often used for file uploads/downloads; may allow anonymous or weakly protected access |
| 22   | SSH    | Secure remote management interface for Linux/Unix systems |
| 23   | Telnet | Legacy remote access protocol, typically unencrypted |
| 25   | SMTP   | Mail transfer service, sometimes exposes user or relay misconfigurations |
| 53   | DNS    | Domain Name System service for name resolution |
| 80   | HTTP   | Unencrypted web service |
| 110  | POP3   | Email retrieval service |
| 139  | SMB    | Windows file sharing over NetBIOS |
| 143  | IMAP   | Email retrieval service with advanced features |
| 443  | HTTPS  | Encrypted web service |
| 445  | SMB    | Windows file sharing over TCP |
| 3306 | MySQL  | Relational database service |
| 3389 | RDP    | Remote Desktop access for Windows systems |
| 5900 | VNC    | Remote graphical desktop service |
| 8080 | HTTP Alt | Alternative web service or proxy interface |

> Note: Open ports should always be reviewed in context to determine their necessity,
> exposure level, and associated security controls.


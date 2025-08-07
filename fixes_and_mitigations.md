# Fixes and Mitigations

## General Recommendations

- Disable services not in use
- Apply latest OS and service patches
- Configure firewalls to restrict access
- Use strong authentication for services like PostgreSQL, SMB, etc.

### Specific Port Fixes

- **Port 135 (MSRPC):** Restrict access via firewall. Disable if not needed.
- **Port 445 (SMB):** Patch Windows with MS17-010 fix. Disable SMBv1.
- **Ports 902/912 (VMware):** Only allow trusted IPs. Keep VMware tools updated.
- **Port 5432 (PostgreSQL):** Enforce strong passwords and IP whitelisting.
- **Port 8080/8443 (Apache):** Ensure latest version is installed. Run SSL test.
- **Port 27000 (FlexLM):** Disable if unused. Protect via firewall/IP filtering.
- **Ports 1042/1043:** Investigate unknown services. Terminate if unnecessary.

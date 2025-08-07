# Identified Vulnerabilities

The following services and ports were found open. Some are known to have historical or potential vulnerabilities:

| Port | Service           | Risk Level | Notes |
|------|-------------------|------------|-------|
| 135  | MSRPC             | Medium     | Can be exploited for information disclosure and lateral movement |
| 445  | Microsoft-DS (SMB)| High       | Often exploited in SMB-based attacks (e.g., EternalBlue - MS17-010) |
| 902  | VMware Auth (SSL) | Medium     | VMware services could be misconfigured or outdated |
| 912  | VMware Auth       | Medium     | May expose management interface |
| 1042 | Unknown (Afrog?)  | Unknown    | Possibly a web service returning 404 - Unrecognized |
| 1043 | Unknown (SSL/Boinc?) | Unknown | Uses SSL, but unrecognized |
| 5432 | PostgreSQL        | Medium     | If exposed without auth, can be vulnerable to SQL injection or takeover |
| 8080 | Apache HTTP       | Medium     | Web server exposed, check for outdated version or misconfig |
| 8443 | Apache HTTPS      | Medium     | SSL-enabled web service, may have SSL/TLS misconfigs |
| 27000| FlexLM            | Medium     | Licensing service, rarely secured |

Use of unrecognized services (1042, 1043) may indicate unnecessary apps running.

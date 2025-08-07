# Critical Vulnerabilities

These are the most critical services found during the scan based on their historical exploitation and CVSS scores.

| Port | Service      | CVE / Vulnerability         | CVSS Score | Severity | Notes |
|------|--------------|-----------------------------|------------|----------|-------|
| 445  | SMB          | MS17-010 (EternalBlue)      | 9.8        | Critical | Used in WannaCry/Ransomware |
| 5432 | PostgreSQL   | CVE-2019-9193               | 7.5        | High     | Bypass via crafted SQL |
| 8080 | Apache HTTP  | CVE-2021-41773 (Path Trav.) | 7.5        | High     | If outdated Apache version |
| 902  | VMware       | CVE-2021-21972              | 9.8        | Critical | Remote code execution in vCenter |
| 135  | MSRPC        | CVE-2021-26414              | 8.1        | High     | RPC Runtime Elevation of Privilege |


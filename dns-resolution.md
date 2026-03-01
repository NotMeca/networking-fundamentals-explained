# DNS Resolution Process

## What is DNS?

DNS (Domain Name System) translates domain names into IP addresses.

## Step-by-Step Process

1. User enters google.com
2. Local cache is checked
3. Request sent to DNS resolver
4. Resolver queries:
   - Root server
   - TLD server
   - Authoritative server
5. IP address returned to client

## Why This Matters in Security

SOC analysts monitor:

- Suspicious domains
- High-frequency DNS queries
- DNS tunneling attempts
- Communication with malicious C2 domains

## Common Port

DNS typically uses:

- Port 53 (UDP)
- Port 53 (TCP for large responses)

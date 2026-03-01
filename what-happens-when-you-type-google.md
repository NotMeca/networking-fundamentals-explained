# What Happens When You Type google.com

1. Browser checks local cache
2. DNS resolution occurs (Port 53)
3. TCP handshake begins (Port 443 for HTTPS)
4. TLS handshake establishes encryption
5. HTTP request is sent
6. Server responds with webpage data

## Security Perspective

A SOC analyst might check:

- Destination IP reputation
- TLS certificate validity
- Suspicious outbound traffic
- Unusual ports used for web traffic

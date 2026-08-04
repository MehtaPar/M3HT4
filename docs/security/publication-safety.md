# Publication Safety Standard

M3HT4 is designed to be publicly useful without exposing the live environment.

## Classification

### Public

- Sanitized architecture
- Generic configuration examples
- Lessons learned
- Detection rules
- Automation
- Technology rationale
- Portfolio case studies

### Private operational

- Real internal addressing
- Hostnames and inventory
- Detailed topology
- Maintenance history
- Environment-specific recovery commands

### Secret

- Credentials
- Tokens
- Private keys
- Recovery codes
- VPN secrets
- Certificate private keys
- Authentication databases

Secrets belong in a password manager or secrets vault—not Git.

## Screenshot checklist

Before publishing:

- Review browser tabs and address bars
- Hide usernames and notifications
- Remove unnecessary hostnames, IPs, MACs, serials, and UUIDs
- Inspect QR codes and barcodes
- Check terminal history and command arguments
- Hide public origin endpoints and management URLs
- Remove tokens, cookies, keys, and certificate material

# Public Repository Threat Model

## Assets to protect

- Home network
- Management interfaces
- Firewall and VPN access
- Identity infrastructure
- Backup locations
- Hosting and DNS control
- Personal account information

## Threats

- Reconnaissance from public documentation
- Accidental secret commits
- Screenshots exposing operational details
- Public diagrams revealing exploitable trust paths
- Repository history retaining deleted secrets
- Website deployment exposing the home-lab origin

## Controls

- Sanitized examples and diagrams
- Separate public and private repositories
- Secret-pattern checks
- No direct hosting from the home lab
- No public management endpoints
- Review screenshots before publication
- Rotate exposed secrets rather than merely deleting them

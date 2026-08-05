# Publication Safety

This repository is public. Contributions must be reviewed for security, privacy, legal, and licensing concerns before they are pushed.

## Never publish

- Credentials, passwords, tokens, recovery codes, or authentication cookies.
- Private keys, certificates containing private material, or VPN secrets.
- Live public endpoints or firewall/NAT rules that expose services.
- Real internal addressing combined with detailed topology or management paths.
- Device serial numbers, account identifiers, or environment-specific access details.
- Raw private captures, logs, screenshots, or exports containing sensitive information.
- Proprietary code, restricted material, or third-party content without appropriate permission.

## Public-safe alternatives

- Use placeholders and generalized diagrams.
- Publish sanitized excerpts rather than raw exports.
- Describe architecture logically rather than reproducing the live environment.
- Use fictional example values and clearly label them.
- Record third-party licenses and attribution where required.

## Before a public commit

1. Review every changed file in GitHub Desktop.
2. Confirm GitHub secret scanning and push protection report no issues.
3. Search for credentials, internal identifiers, addresses, and private endpoints.
4. Confirm images do not reveal browser tabs, account names, QR codes, or infrastructure details.
5. Verify licensing and attribution.
6. Confirm wording matches the current M3HT4 vision.

# Publication Safety Standard

M3HT4 is a public repository. Every contribution must be reviewed as though it will be indexed, copied, and retained permanently.

## Safe to publish

- generalized architectures and diagrams;
- sanitized scenario descriptions;
- placeholder addressing and identifiers;
- vendor-neutral workflows;
- original content or properly licensed resources;
- lessons learned without identifying private systems or people.

## Keep private

- credentials, tokens, API keys, private keys, and recovery codes;
- authentication cookies and session material;
- real internal IP addresses, hostnames, domains, UUIDs, MAC addresses, or serial numbers;
- VPN configurations, management paths, or firewall rules that expose access;
- raw private packet captures, memory dumps, backups, or virtual-machine images;
- cloud/account identifiers and private certificates;
- environment-specific details that materially increase risk.

## Example placeholders

```text
host.example.lab
192.0.2.10
AA:BB:CC:XX:XX:XX
<REDACTED_UUID>
<REDACTED_TOKEN>
```

## Before publishing

1. Review every changed file and image.
2. Confirm no secret-scanning alerts are present.
3. Search for environment-specific names and addresses.
4. Confirm third-party code, data, and media are appropriately licensed.
5. Verify the content supports the public M3HT4 vision.
6. When uncertain, keep the information private until reviewed.

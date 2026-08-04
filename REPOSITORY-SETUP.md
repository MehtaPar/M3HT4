# GitHub Repository Setup

After committing this upgrade:

## About section

- Description: `M3HT4 — Modern • Managed • Multi-Domain cyber range for blue-team defense, red-team testing, and Hybrid Threat Hunting & Training.`
- Website: `https://www.m3ht4.com`
- Topics:
  - cybersecurity
  - cyber-range
  - threat-hunting
  - detection-engineering
  - adversary-emulation
  - proxmox
  - opnsense
  - active-directory
  - homelab
  - security-automation

## Social preview

Upload:

```text
assets/branding/m3ht4-social-preview.png
```

under:

```text
Settings → General → Social preview
```

## GitHub Pages

After replacing `OWNER` placeholders:

1. Push the repository.
2. Open **Settings → Pages**.
3. Set deployment source to **Deploy from a branch**.
4. Select the `gh-pages` branch after the documentation workflow runs.
5. Use `/ (root)`.

Do not point M3HT4.com at GitHub Pages until DNS and hosting decisions are finalized.

## Security

Enable where available:

- Secret scanning
- Push protection
- Dependabot alerts
- Private vulnerability reporting
- Branch protection for `main`

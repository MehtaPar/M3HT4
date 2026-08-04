# M3HT4.com

M3HT4.com will be the public-facing home of the project.

## Site goals

- Explain M3HT4 clearly to technical and non-technical visitors
- Showcase sanitized architecture and project milestones
- Publish detection, hunting, and analytics case studies
- Link directly to reusable public repository content
- Provide a polished portfolio experience

## Recommended sections

1. Home
2. Architecture
3. Projects
4. Detection Engineering
5. Threat Hunting
6. Roadmap
7. About

## Deployment boundary

The public website should be deployed separately from the home lab.

Recommended:

- Static or managed hosting
- HTTPS
- No direct home-lab origin exposure
- No inbound port forwarding to management systems
- No Proxmox, OPNsense, iDRAC, or switch interface exposure
- Provider secrets stored outside Git

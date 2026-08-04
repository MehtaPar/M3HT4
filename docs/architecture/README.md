# Architecture

M3HT4 is designed as a segmented, recoverable cyber range rather than a flat collection of systems.

## Architecture principles

- Separate management from testing traffic
- Keep offensive tooling isolated from household and management systems
- Treat backups as an independent recovery layer
- Use dedicated infrastructure roles where practical
- Prefer clear trust boundaries over unnecessary complexity
- Avoid exposing management services publicly
- Document the design without publishing the live implementation

## Views

| View | Purpose |
|---|---|
| [Physical topology](physical-topology.md) | Hardware roles and high-level connectivity |
| [Logical topology](logical-topology.md) | Services and security zones |
| [Storage architecture](storage-layout.md) | Host, VM, infrastructure, and backup separation |
| [Trust boundaries](trust-boundaries.md) | Planned isolation and traffic-control model |

```mermaid
flowchart LR
    Physical[Physical Platform] --> Virtual[Virtualization]
    Virtual --> Services[Identity and Core Services]
    Services --> Telemetry[Detection and Analytics]
    Telemetry --> Validation[Adversary Emulation]
    Validation --> Improvement[Automation and Continuous Improvement]
```

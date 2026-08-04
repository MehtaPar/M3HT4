# Trust Boundaries

M3HT4 treats network placement as a security control.

| Zone | Trust level | Typical systems | Primary restrictions |
|---|---|---|---|
| Management | Highest | Hypervisor, switch, firewall management | Restricted administrator access |
| Servers | High | Identity and internal services | Limited inbound access |
| Monitoring | High | SIEM, sensors, analytics | Broad visibility, limited control paths |
| Endpoints | Medium | Windows and Linux clients | User-oriented access |
| Offensive | Low | Attack tooling and emulation systems | Isolated, controlled egress |
| DMZ | Low | Deliberately exposed lab services | No implicit trust to internal systems |
| Guest / IoT | Untrusted | Household and test devices | Internet-oriented access only |

The live firewall rules and real network implementation are intentionally private.

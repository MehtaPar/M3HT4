# Physical Topology

The public topology uses generic roles and intentionally omits live interfaces, port numbers, serial numbers, internal addresses, and management endpoints.

```mermaid
flowchart TB
    ISP[ISP Gateway / Modem]
    FW[Dedicated Firewall Appliance]
    CORE[Managed Core Switch]
    HYP[Virtualization Server]
    ADMIN[Administrative Workstation]
    REMOTE[Secure Remote Administration]
    BACKUP[(Independent Backup Storage)]

    ISP --> FW
    FW --> CORE
    CORE --> HYP
    CORE --> ADMIN
    HYP --> BACKUP
    REMOTE -. Authenticated administration .-> FW
```

## Role summary

| Component | Role |
|---|---|
| Firewall appliance | Routing, policy enforcement, segmentation, VPN |
| Managed switch | VLAN distribution and wired access |
| Virtualization server | Hosts identity, endpoints, monitoring, and lab systems |
| Administrative workstation | Restricted management and engineering |
| Backup storage | Independent VM and configuration recovery |

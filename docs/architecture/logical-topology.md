# Logical Topology

```mermaid
flowchart LR
    Firewall[Firewall and Routing]

    subgraph Zones["Security Zones"]
        Mgmt[Management]
        Servers[Servers]
        Endpoints[Endpoints]
        Offensive[Authorized Offensive]
        Monitoring[Monitoring]
        DMZ[DMZ]
        Guest[Guest / IoT]
    end

    Firewall --> Mgmt
    Firewall --> Servers
    Firewall --> Endpoints
    Firewall --> Offensive
    Firewall --> Monitoring
    Firewall --> DMZ
    Firewall --> Guest

    Servers --> Identity[Identity and DNS]
    Monitoring --> SIEM[SIEM and Network Analytics]
    Offensive --> Range[Controlled Targets]
```

## Planned controls

- Default-deny inter-zone policy
- Explicit management access paths
- Restricted offensive-zone egress
- No direct management exposure to the Internet
- Logging at trust-boundary crossings
- Separate public hosting from the home lab

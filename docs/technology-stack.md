# Technology Strategy

M3HT4 selects technologies based on operational value and learning objectives.

| Capability | Technology direction | Purpose |
|---|---|---|
| Virtualization | Proxmox VE, QEMU/KVM | Workload lifecycle and isolation |
| Storage | LVM-Thin, independent backups | Flexible VM storage and recovery |
| Identity | Windows Server, AD DS, DNS | Enterprise identity workflows |
| Firewalling | OPNsense | Segmentation, policy, VPN, visibility |
| Switching | Managed Ethernet and VLANs | Trust-zone implementation |
| Endpoints | Windows, Linux, Kali | User, server, blue-team, and red-team roles |
| Offensive security | Kali, controlled targets, pentest tooling | Authorized reconnaissance, exploitation, post-exploitation, and reporting |
| Endpoint telemetry | Sysmon, WEF | High-value Windows visibility |
| Network telemetry | Zeek, Suricata | Metadata and IDS coverage |
| SIEM | Wazuh / compatible stack | Central analysis and alerting |
| Purple-team validation | MITRE ATT&CK mapping and controlled exercises | Verify telemetry and detection coverage |
| Analytics | Python, Jupyter | Repeatable threat-hunting analysis |
| Automation | Bash, PowerShell, Python | Reduce manual operations |
| AI assistance | Local models | Triage, documentation, and analysis support |

## Selection rule

A tool is added only when it supports a defined outcome such as:

- Better visibility
- Better recovery
- More realistic enterprise workflows
- Repeatable validation
- Measurable learning


## Dual-team design goal

M3HT4 is designed so that offensive workflows generate meaningful defensive telemetry. Red-team activities should be observable, blue-team controls should be testable, and both sides should contribute to repeatable purple-team exercises.

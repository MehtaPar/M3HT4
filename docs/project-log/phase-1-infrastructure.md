# Phase 1 — Infrastructure v1.0

## Mission

Build a clean, recoverable virtualization foundation before adding enterprise networking and security tooling.

## Deliverables

- Fresh Proxmox deployment
- Dedicated boot, VM, infrastructure, and backup storage roles
- Storage sanitization appropriate to device capabilities
- Identity-services VM backup
- SHA-256 integrity validation
- Hypervisor rebuild
- Existing datastore registration
- Successful VM restoration
- Golden recovery snapshot
- Automated independent backups

## Recovery validation

```mermaid
flowchart LR
    Backup[Verified VM Backup]
    Rebuild[Fresh Hypervisor]
    Storage[Datastores Registered]
    Restore[Critical VM Restored]
    Validate[Services Validated]
    Protect[Snapshot and Scheduled Backup]

    Backup --> Rebuild --> Storage --> Restore --> Validate --> Protect
```

## Engineering lessons

- Device capabilities must be verified rather than assumed
- Logical overwrite and controller-level sanitization are not identical
- Hardware should be identified by persistent identifiers
- Recovery testing often reveals compatibility issues documentation alone misses
- Operational safety and publication safety should be designed together
- Stable infrastructure is more valuable than premature complexity

# Backup and Recovery

M3HT4 uses complementary recovery layers.

| Layer | Purpose |
|---|---|
| Snapshot | Rapid rollback before risky changes |
| Independent backup | Recovery from VM, datastore, or host failure |
| Documentation | Repeatable rebuild and validation |
| Restore test | Proof that the backup actually works |

```mermaid
sequenceDiagram
    participant Backup as Independent Backup
    participant Host as Fresh Hypervisor
    participant Store as VM Datastore
    participant VM as Restored Workload

    Host->>Store: Register existing datastore
    Host->>Backup: Mount backup repository
    Backup->>Host: Restore compressed VM archive
    Host->>VM: Start workload
    VM-->>Host: Validate identity, DNS, and networking
    Host->>VM: Create known-good snapshot
    Host->>Backup: Run fresh backup
```

## Validated result

The infrastructure milestone included a successful end-to-end recovery:

1. Hypervisor rebuilt
2. Storage re-registered
3. Backup repository mounted
4. Critical VM restored
5. Compatibility issue resolved
6. Workload started and validated
7. New snapshot created
8. Automated backup completed successfully

# Storage Architecture

```mermaid
flowchart LR
    BOOT[(Boot Storage)]
    VM[(Primary VM Datastore)]
    INFRA[(Infrastructure Library)]
    BAK[(Independent Backup Storage)]

    BOOT --> HOST[Hypervisor OS and host configuration]
    VM --> WORKLOADS[VM disks, containers, snapshots]
    INFRA --> CONTENT[ISOs, templates, drivers, snippets]
    BAK --> RECOVERY[Compressed VM backups and recovery artifacts]
```

## Design rationale

| Tier | Purpose | Recovery expectation |
|---|---|---|
| Boot | Hypervisor OS and configuration | Reinstallable |
| VM datastore | Active workloads | Protected by backup |
| Infrastructure | Installation media and reusable content | Rebuildable |
| Backup | Independent recovery archives | Critical |

This separation prevents active workloads from depending on the boot disk and makes host recovery significantly simpler.

# Reference Architecture

M3HT4 separates the public product from the private environment used to validate it.

```mermaid
flowchart LR
    Lab[Private validation environment] --> Artifacts[Sanitized evidence and reusable artifacts]
    Artifacts --> Framework[Public M3HT4 framework]
    Framework --> Web[Future interactive platform]
    Web --> Users[Blue · Red · Purple teams]

    classDef private fill:#3a1720,stroke:#ff5d73,color:#fff;
    classDef public fill:#092b46,stroke:#15b8ff,color:#fff;
    class Lab private;
    class Artifacts,Framework,Web,Users public;
```

## Layer 1: Private validation environment

Used to test assumptions, generate controlled evidence, and validate workflows. Configuration details remain private unless they are intentionally generalized and safe to publish.

## Layer 2: Sanitized artifacts

Representative logs, diagrams, templates, mappings, and lessons learned are reviewed before publication.

## Layer 3: Public framework

Documentation and reusable workflows connect behavior, evidence, hunting, detection, emulation, and learning.

## Layer 4: Interactive platform

M3HT4.com will eventually guide users through framework content and scenario workflows without exposing the private validation environment.

## Boundary rule

No public feature should require the publication of credentials, live addressing, sensitive topology, private endpoints, firewall policy, authentication material, raw private captures, or operational secrets.

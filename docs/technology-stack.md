# Technology Strategy

M3HT4 is a framework first and a tool stack second. Technologies are selected to support realistic evidence, repeatable workflows, maintainability, and public safety.

## Selection principles

1. **Use the simplest tool that proves the workflow.**
2. **Prefer open standards and exportable formats.**
3. **Avoid locking public content to one vendor.**
4. **Separate private infrastructure from the public application.**
5. **Choose licenses compatible with open-source and potential commercial use.**
6. **Keep operating costs appropriate for a small project.**
7. **Treat AI as optional internal assistance, not a source of truth.**

## Technology layers

| Layer | Current direction | Role in M3HT4 |
|---|---|---|
| Validation environment | Virtualized Windows and Linux systems | Safely generate and verify representative behavior and evidence |
| Identity and networking | Directory services, segmented networks, controlled routing | Support realistic identity, endpoint, and network scenarios |
| Telemetry | Native logs plus open or widely supported sensors | Provide evidence for hunting, detection, and validation |
| Analytics | Python and notebooks where useful | Explore data and prototype repeatable analysis |
| Content | Markdown, JSON/YAML schemas, sanitized sample data | Keep scenarios portable and reviewable |
| Documentation | GitHub and MkDocs | Publish professional, searchable public documentation |
| Web application | Lightweight, managed hosting | Deliver the interactive framework without exposing the private lab |
| Automation | Python, PowerShell, shell scripts, APIs | Reduce repetitive preparation and validation work |

## Vendor-neutrality

Vendor-neutral does not mean avoiding named products. It means that the durable value of M3HT4 should live in:

- the question being asked;
- the behavior being examined;
- the evidence required;
- the analysis method;
- the engagement design;
- the resulting improvement.

Tool-specific examples may be included when useful, but core scenarios should explain transferable concepts and clearly label vendor-specific dependencies.

## AI use

AI tools may assist privately with drafting, coding, summarization, or exploring ideas. They should not:

- generate unreviewed public conclusions;
- be presented as a required platform dependency;
- replace evidence-based analysis;
- introduce proprietary or ambiguously licensed material;
- receive credentials, private captures, or sensitive environment details.

## Licensing and legal hygiene

Before including third-party code, data, images, or documentation:

- confirm the license and attribution requirements;
- avoid copying proprietary training content or commercial datasets;
- prefer original examples and openly licensed resources;
- preserve required notices;
- document important dependencies.

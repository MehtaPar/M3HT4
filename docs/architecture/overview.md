# M3HT4 Reference Architecture

## Architectural purpose

The architecture separates the **public framework** from the **private validation environment**.

| Layer | Purpose | Public? |
|---|---|:---:|
| Public repository | Vision, documentation, templates, sanitized scenarios | Yes |
| Future web platform | Guided workflows and interactive framework experience | Yes |
| Validation environment | Generates and verifies representative evidence | No |
| Private operations | Credentials, addressing, management, backups, access paths | No |

## Logical flow

1. A scenario is designed using public-safe objectives and assumptions.
2. Representative activity is tested in an authorized private environment.
3. Resulting evidence is reviewed and sanitized.
4. Reusable workflows and lessons are published publicly.
5. The public framework remains useful without exposing the private environment.

## Design principles

- **Separation:** public documentation never depends on revealing real internal details.
- **Sanitization:** examples use placeholders and generalized diagrams.
- **Portability:** workflows should remain useful across products and environments.
- **Maintainability:** the project favors a small number of validated patterns.
- **Traceability:** published artifacts explain assumptions, evidence, limitations, and outcomes.

> [!IMPORTANT]
> The reference environment supports M3HT4 development. It is not the M3HT4 product itself.

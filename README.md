<p align="center">
  <img src="assets/branding/m3ht4-banner.png" alt="M3HT4 — Modern Hunting Terrain" width="100%">
</p>

<h1 align="center">M3HT4 — Modern Hunting Terrain</h1>

<p align="center">
  <strong>An interactive cybersecurity framework for Blue, Red, and Purple teams.</strong><br>
  Learn the data. Hunt the behavior. Plan the emulation. Improve together.
</p>

<p align="center">
  <a href="docs/framework/vision.md"><img alt="Platform Vision" src="https://img.shields.io/badge/Platform-Vision-15b8ff?style=for-the-badge&logo=readthedocs&logoColor=white"></a>
  <a href="docs/framework/operating-model.md"><img alt="3 Teams" src="https://img.shields.io/badge/3-Teams-8b5cf6?style=for-the-badge&logo=teamspeak&logoColor=white"></a>
  <a href="docs/framework/operating-model.md#the-four-pillars"><img alt="4 Pillars" src="https://img.shields.io/badge/4-Pillars-00b894?style=for-the-badge&logo=target&logoColor=white"></a>
  <a href="docs/roadmap/roadmap.md"><img alt="Roadmap" src="https://img.shields.io/badge/View-Roadmap-f59e0b?style=for-the-badge&logo=roadmap&logoColor=white"></a>
  <a href="docs/roadmap/status.md"><img alt="Project Status" src="https://img.shields.io/badge/Project-Status-ff5d73?style=for-the-badge&logo=statuspage&logoColor=white"></a>
  <a href="docs/README.md"><img alt="Documentation" src="https://img.shields.io/badge/Open-Documentation-326ce5?style=for-the-badge&logo=gitbook&logoColor=white"></a>
</p>

> [!WARNING]
> **M3HT4 is under active development.** The framework, documentation, examples, and reference environment are being built incrementally. Current material represents the project direction—not a finished production platform. Expect the structure and examples to evolve as end-to-end scenarios are validated.

<p align="center">
  <img alt="Development stage" src="https://img.shields.io/badge/Stage-Early%20Development-f59e0b?style=flat-square">
  <img alt="Public repository" src="https://img.shields.io/badge/Repository-Public%20%26%20Sanitized-00b894?style=flat-square">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-2563eb?style=flat-square">
  <img alt="Use" src="https://img.shields.io/badge/Use-Authorized%20Security%20Work-8b5cf6?style=flat-square">
</p>

---

## What is M3HT4?

**M3HT4 (Modern Hunting Terrain)** is a developing cybersecurity framework that helps **Blue, Red, and Purple teams** build a shared understanding of security data, threat hunting, adversary behavior, and engagement planning.

The goal is not to become an enormous repository of every CVE, threat actor, or technique. M3HT4 is designed to remain a **curated, lightweight, and maintainable framework** that connects realistic evidence to repeatable workflows.

- **Blue teams** use representative telemetry to investigate behavior, test hypotheses, and improve detections.
- **Red teams** study defender visibility and turn objectives into safe, evidence-aware adversary-emulation plans.
- **Purple teams** connect offensive intent with defensive evidence to design engagements, validate coverage, and document improvements.

<p align="center"><strong>Built for 3 Teams. Powered by 4 Pillars.</strong></p>

<p align="center">
  <img src="assets/diagrams/m3ht4-framework.svg" alt="M3HT4 framework connecting three teams and four pillars" width="940">
</p>

---

## Explore M3HT4

<table>
<tr>
<td width="50%"><a href="docs/framework/vision.md"><img src="assets/cards/vision.svg" alt="Platform Vision"></a></td>
<td width="50%"><a href="docs/framework/operating-model.md"><img src="assets/cards/teams.svg" alt="Three Teams"></a></td>
</tr>
<tr>
<td width="50%"><a href="docs/framework/operating-model.md#the-four-pillars"><img src="assets/cards/pillars.svg" alt="Four Pillars"></a></td>
<td width="50%"><a href="docs/roadmap/roadmap.md"><img src="assets/cards/roadmap.svg" alt="Roadmap"></a></td>
</tr>
<tr>
<td width="50%"><a href="docs/roadmap/status.md"><img src="assets/cards/status.svg" alt="Project Status"></a></td>
<td width="50%"><a href="docs/README.md"><img src="assets/cards/docs.svg" alt="Documentation"></a></td>
</tr>
</table>

---

## The 3 Teams

| Team | Perspective | How M3HT4 helps |
|:---:|---|---|
| 🔵 **Blue Team** | Observe, investigate, detect, and respond | Build familiarity with telemetry, develop hunt logic, validate visibility, and convert findings into defensible improvements |
| 🔴 **Red Team** | Understand and emulate adversary behavior | Build realistic plans around objectives, expected evidence, safety controls, and defender visibility |
| 🟣 **Purple Team** | Coordinate offense and defense | Connect intent, activity, evidence, detections, and lessons learned into a measurable engagement loop |

## The 4 Pillars

| Pillar | Purpose | Representative output |
|:---:|---|---|
| 🔎 **Hunt** | Explore telemetry and test investigative hypotheses | Hunt plans, timelines, findings, pivots, and unanswered questions |
| 🛡️ **Detect** | Convert observed behavior into reusable defensive logic | Detection ideas, mappings, test evidence, and tuning notes |
| ♟️ **Emulate** | Plan safe, authorized adversary behavior against clear objectives | Emulation plans, expected telemetry, guardrails, and success criteria |
| 📘 **Train** | Build practical understanding through guided, repeatable use | Exercises, walkthroughs, analyst notes, and lessons learned |

<p align="center">
  <img src="assets/diagrams/team-pillar-loop.svg" alt="M3HT4 team and pillar collaboration loop" width="900">
</p>

---

## How the framework works

```mermaid
flowchart LR
    R[Red Team<br/>Plans authorized emulation] --> A[Controlled activity<br/>and expected evidence]
    A --> B[Blue Team<br/>Hunts and validates visibility]
    B --> P[Purple Team<br/>Compares intent, evidence, and outcome]
    P --> I[Improvements<br/>Detections · Plans · Procedures · Learning]
    I --> R
```

A scenario should create value for all three teams. The red-team plan defines intended behavior. The blue team examines the resulting evidence. The purple team compares expectations with reality and turns gaps into concrete improvements.

---

## What the project will deliver

M3HT4 is being developed in layers:

1. **Safe reference environment** — generate and validate realistic, controlled security evidence.
2. **Curated knowledge model** — connect behavior, telemetry, hunting questions, detections, and emulation planning.
3. **Interactive platform** — guide users through scenarios without exposing or requiring access to the private lab.
4. **Reusable public artifacts** — provide sanitized templates, examples, walkthroughs, and case studies.

> [!NOTE]
> The private reference lab supports development and validation, but **the lab is not the product**. The public framework should remain useful without revealing private infrastructure.

## Current progress

| Workstream | Status |
|---|:---:|
| Refined identity and framework vision | ✅ Established |
| Public documentation structure | 🟡 In progress |
| Safe validation environment | 🟡 In progress |
| First telemetry and hunting workflow | 🔵 Planned |
| First adversary-emulation planning workflow | 🔵 Planned |
| First complete purple-team scenario | 🔵 Planned |
| Interactive M3HT4 web application | 🔵 Planned |

<p align="center">
  <a href="docs/roadmap/status.md"><img alt="Detailed Status" src="https://img.shields.io/badge/View-Detailed%20Status-ff5d73?style=for-the-badge&logo=statuspage&logoColor=white"></a>
  <a href="docs/roadmap/roadmap.md"><img alt="Delivery Roadmap" src="https://img.shields.io/badge/View-Delivery%20Roadmap-f59e0b?style=for-the-badge&logo=roadmap&logoColor=white"></a>
</p>

<p align="center">
  <img src="assets/diagrams/roadmap.svg" alt="M3HT4 phased roadmap" width="940">
</p>

---

## Scope and guardrails

M3HT4 is intended for **authorized** defensive analysis, detection validation, threat hunting, adversary-emulation planning, security research, and education.

Public material emphasizes sanitized examples, behavior and evidence over exploit novelty, safe planning and validation, vendor-neutral concepts where practical, and a strict separation between public documentation and private operations.

> [!CAUTION]
> Use M3HT4 only with systems you own or are explicitly authorized to test. The framework is designed to improve collaboration and controlled validation—not to enable unauthorized access.

## Documentation map

| Start here | Description |
|---|---|
| [Documentation hub](docs/README.md) | Organized entry point for all project documentation |
| [Platform vision](docs/framework/vision.md) | Product definition, users, boundaries, and long-term direction |
| [Operating model](docs/framework/operating-model.md) | How the three teams use the four pillars together |
| [Architecture](docs/architecture/reference-architecture.md) | Public-safe logical model and separation boundaries |
| [Project status](docs/roadmap/status.md) | Current progress and immediate next milestone |
| [Roadmap](docs/roadmap/roadmap.md) | Incremental delivery phases and sequencing |
| [Technology strategy](docs/architecture/technology-strategy.md) | Selection principles without unnecessary vendor lock-in |
| [M3HT4.com plan](website/README.md) | Public website and future interactive application direction |

## Repository structure

```text
M3HT4/
├── .github/                  Workflows and community templates
├── assets/                   Branding, cards, and public-safe diagrams
├── docs/                     Vision, model, architecture, and roadmap
├── examples/                 Sanitized scenario templates and future examples
├── website/                  M3HT4.com product direction
├── mkdocs.yml                Documentation-site configuration
└── README.md                 Public project landing page
```

## Development principles

- Build one useful, validated workflow before expanding the catalog.
- Prefer curated depth over an unmaintainable data dump.
- Make every feature support at least one team and one pillar.
- Keep public content separate from private infrastructure.
- Use automation to reduce repetitive work—not to replace analyst judgment.
- Document assumptions, evidence, limitations, and lessons learned.
- Favor simple, maintainable architecture that a small team can operate.

---

<p align="center">
  <strong>One terrain. Three teams. Four paths to improvement.</strong><br>
  <em>Build. Defend. Hunt. Evolve.</em>
</p>

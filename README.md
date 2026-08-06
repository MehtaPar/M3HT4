<p align="center">
  <img src="assets/branding/m3ht4-banner.jpg" alt="M3HT4 — Modern Hunting Terrain" width="100%">
</p>

<h1 align="center">M3HT4 — Modern Hunting Terrain</h1>

<p align="center">
  <strong>An interactive cybersecurity framework for Blue, Red, and Purple teams.</strong><br>
  Learn the data. Hunt the behavior. Plan the emulation. Improve together.
</p>

<p align="center">
  <a href="docs/framework/vision.md"><img alt="Platform vision" src="https://img.shields.io/badge/Platform-Vision-15b8ff?style=for-the-badge"></a>
  <a href="docs/framework/operating-model.md"><img alt="Three teams" src="https://img.shields.io/badge/3-Teams-8b5cf6?style=for-the-badge"></a>
  <a href="docs/framework/operating-model.md#the-four-pillars"><img alt="Four pillars" src="https://img.shields.io/badge/4-Pillars-00b894?style=for-the-badge"></a>
  <a href="docs/roadmap/roadmap.md"><img alt="Roadmap" src="https://img.shields.io/badge/View-Roadmap-f59e0b?style=for-the-badge"></a>
  <a href="docs/roadmap/status.md"><img alt="Project status" src="https://img.shields.io/badge/Project-Status-ff5d73?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="docs/roadmap/status.md"><img alt="Early development" src="https://img.shields.io/badge/Stage-Early%20Development-f59e0b?style=flat-square"></a>
  <a href="docs/security/publication-safety.md"><img alt="Public and sanitized" src="https://img.shields.io/badge/Repository-Public%20%26%20Sanitized-00b894?style=flat-square"></a>
  <a href="LICENSE"><img alt="MIT license" src="https://img.shields.io/badge/License-MIT-2563eb?style=flat-square"></a>
  <a href="SECURITY.md"><img alt="Authorized security work" src="https://img.shields.io/badge/Use-Authorized%20Security%20Work-8b5cf6?style=flat-square"></a>
</p>

> [!WARNING]
> **M3HT4 is under active development.** The public framework, documentation, examples, and private reference environment are being built incrementally. Current material represents the validated direction of the project—not a finished production platform.

---

## What is M3HT4?

**M3HT4 (Modern Hunting Terrain)** is a curated cybersecurity framework that helps **Blue, Red, and Purple teams** understand the same security data, connect adversary behavior to defender-visible evidence, and build stronger threat-hunting and engagement plans.

The framework is intentionally designed to remain:

- **curated** rather than becoming a massive CVE or threat-data dump;
- **lightweight** enough for a small team to maintain;
- **vendor-neutral** where practical;
- **public-safe** and separated from private infrastructure;
- **useful across perspectives**, not limited to one role or tool.

<p align="center"><strong>Built for 3 Teams. Powered by 4 Pillars.</strong></p>

```mermaid
flowchart TB
    M["M3HT4<br/>Modern Hunting Terrain"]

    subgraph T["Built for 3 Teams"]
      B["🔵 Blue Team<br/>Observe · Hunt · Detect"]
      R["🔴 Red Team<br/>Understand · Plan · Emulate"]
      P["🟣 Purple Team<br/>Align · Validate · Improve"]
    end

    subgraph F["Powered by 4 Pillars"]
      H["🔎 Hunt"]
      D["🛡️ Detect"]
      E["♟️ Emulate"]
      TR["📘 Train"]
    end

    M --> B
    M --> R
    M --> P
    B --> H
    B --> D
    R --> E
    R --> TR
    P --> H
    P --> D
    P --> E
    P --> TR

    classDef core fill:#101827,stroke:#15b8ff,color:#ffffff,stroke-width:3px;
    classDef blue fill:#0b3b70,stroke:#32a4ff,color:#ffffff;
    classDef red fill:#651d2b,stroke:#ff5d73,color:#ffffff;
    classDef purple fill:#4a216d,stroke:#b267ff,color:#ffffff;
    classDef pillar fill:#102b34,stroke:#26d0ce,color:#ffffff;

    class M core;
    class B blue;
    class R red;
    class P purple;
    class H,D,E,TR pillar;
```

---

## Explore the framework

| Area | What you will find |
|---|---|
| **[🎯 Platform Vision](docs/framework/vision.md)** | Purpose, audience, boundaries, value, and long-term direction |
| **[🔵🔴🟣 Operating Model](docs/framework/operating-model.md)** | How the 3 Teams use the 4 Pillars together |
| **[🏗️ Reference Architecture](docs/architecture/reference-architecture.md)** | Public framework, private validation environment, and information boundaries |
| **[🗺️ Delivery Roadmap](docs/roadmap/roadmap.md)** | Phased implementation designed to avoid unnecessary complexity |
| **[🚧 Project Status](docs/roadmap/status.md)** | What is established, in progress, planned, and intentionally deferred |
| **[🔐 Publication Safety](docs/security/publication-safety.md)** | What may be published and what must remain private |
| **[🧪 Sanitized Examples](examples/README.md)** | Standards and planned structure for public scenarios |
| **[🌐 M3HT4.com Direction](website/README.md)** | How the website and future interactive platform fit the project |

---

## The 3 Teams

| Team | Perspective | How M3HT4 adds value |
|:---:|---|---|
| 🔵 **Blue Team** | Observe, investigate, detect, and respond | Learn representative telemetry, build hunt hypotheses, validate visibility, and improve detections |
| 🔴 **Red Team** | Understand and emulate adversary behavior | Build safe, evidence-aware emulation plans around objectives, guardrails, and expected defender visibility |
| 🟣 **Purple Team** | Coordinate offense and defense | Connect intent, activity, evidence, detections, and lessons into a measurable engagement loop |

## The 4 Pillars

| Pillar | Purpose | Representative output |
|:---:|---|---|
| 🔎 **Hunt** | Explore telemetry and test investigative hypotheses | Hunt plans, pivots, findings, timelines, unanswered questions |
| 🛡️ **Detect** | Convert observed behavior into reusable defensive logic | Detection ideas, mappings, test evidence, tuning notes |
| ♟️ **Emulate** | Plan authorized adversary behavior against clear objectives | Emulation plans, expected evidence, guardrails, success criteria |
| 📘 **Train** | Build practical understanding through guided use | Exercises, walkthroughs, analyst notes, lessons learned |

---

## How M3HT4 creates shared value

```mermaid
sequenceDiagram
    autonumber
    participant R as Red Team
    participant X as Controlled Scenario
    participant B as Blue Team
    participant P as Purple Team
    participant K as Knowledge Base

    R->>X: Define authorized behavior and expected evidence
    X-->>B: Produce representative telemetry
    B->>B: Hunt, investigate, and validate detections
    B-->>P: Share findings, gaps, and confidence
    R-->>P: Share intent, execution notes, and assumptions
    P->>P: Compare expected vs observed outcomes
    P->>K: Record improvements and reusable artifacts
    K-->>R: Improve future emulation plans
    K-->>B: Improve hunts, detections, and procedures
```

A complete scenario should create value for all three teams. Red defines intended behavior, Blue examines evidence, and Purple compares expectations with reality to produce measurable improvements.

<details>
<summary><strong>Example artifact flow</strong></summary>

```mermaid
flowchart LR
    S["Scenario Brief"] --> EP["Emulation Plan"]
    S --> EM["Evidence Map"]
    EP --> TE["Test Execution"]
    TE --> HT["Hunt Timeline"]
    EM --> HT
    HT --> DR["Detection Record"]
    DR --> AAR["After-Action Review"]
    EP --> AAR
    AAR --> BL["Improvement Backlog"]
```

</details>

---

## What the project will deliver

M3HT4 is being developed in layers:

1. **Safe reference environment** — generate and validate realistic, controlled evidence.
2. **Curated knowledge model** — connect behavior, telemetry, hunting questions, detections, and emulation planning.
3. **Reusable public artifacts** — publish sanitized templates, examples, walkthroughs, and case studies.
4. **Interactive platform** — guide users through validated scenarios without exposing the private environment.

> [!NOTE]
> The private reference lab supports development and validation, but **the lab is not the product**. M3HT4 should remain useful without revealing or requiring access to private infrastructure.

## Project Status

| Workstream | Status |
|---|:---:|
| Refined identity and framework vision | ✅ Established |
| 3 Teams / 4 Pillars operating model | ✅ Established |
| Public documentation structure | 🟡 In progress |
| Safe validation environment | 🟡 In progress |
| First end-to-end hunting workflow | 🔵 Planned |
| First adversary-emulation planning workflow | 🔵 Planned |
| First complete Purple-team scenario | 🔵 Planned |
| Interactive M3HT4 web application | 🔵 Planned |

```mermaid
gantt
    title M3HT4 Delivery Sequence
    dateFormat  YYYY-MM-DD
    axisFormat  %b %Y

    section Foundation
    Identity and framework definition    :done, f1, 2026-08-01, 14d
    Public documentation baseline        :active, f2, 2026-08-08, 30d

    section Validation
    First evidence-centered scenario     :v1, after f2, 45d
    Reusable artifact templates          :v2, after v1, 30d

    section Platform
    Curated scenario library             :p1, after v2, 60d
    Interactive application prototype    :p2, after p1, 90d
```

<p align="center">
  <a href="docs/roadmap/status.md"><img alt="Detailed status" src="https://img.shields.io/badge/View-Detailed%20Status-ff5d73?style=for-the-badge"></a>
  <a href="docs/roadmap/roadmap.md"><img alt="Delivery roadmap" src="https://img.shields.io/badge/View-Delivery%20Roadmap-f59e0b?style=for-the-badge"></a>
</p>

---

## Scope and guardrails

M3HT4 is intended for **authorized** defensive analysis, detection validation, threat hunting, adversary-emulation planning, security research, and education.

> [!CAUTION]
> Use M3HT4 only on systems you own or are explicitly authorized to assess. The framework is designed to support collaboration and controlled validation—not unauthorized access or harmful activity.

Public content emphasizes:

- sanitized examples;
- behavior and evidence over exploit novelty;
- safe planning and validation;
- vendor-neutral concepts where practical;
- original or properly licensed materials;
- strict separation between public documentation and private operations.

---

## Documentation map

| Start here | Description |
|---|---|
| [Documentation hub](docs/README.md) | Organized entry point for the public framework |
| [Platform vision](docs/framework/vision.md) | Product definition, audience, boundaries, and long-term direction |
| [Operating model](docs/framework/operating-model.md) | How the 3 Teams and 4 Pillars work together |
| [Reference architecture](docs/architecture/reference-architecture.md) | Public-safe architecture and separation boundaries |
| [Project status](docs/roadmap/status.md) | Current progress and immediate next milestone |
| [Roadmap](docs/roadmap/roadmap.md) | Incremental delivery phases |
| [Technology strategy](docs/architecture/technology-strategy.md) | Selection principles and sustainability |
| [Publication safety](docs/security/publication-safety.md) | Public-release rules |
| [M3HT4.com plan](website/README.md) | Website and future application direction |

## Repository structure

```text
M3HT4/
├── .github/                  Workflows and community templates
├── assets/                   Public branding assets
├── docs/
│   ├── framework/            Vision and operating model
│   ├── architecture/         Reference architecture and technology strategy
│   ├── roadmap/              Status and phased delivery plan
│   └── security/             Publication-safety rules
├── examples/                 Sanitized scenario guidance
├── website/                  M3HT4.com direction
├── mkdocs.yml                Documentation navigation
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
  <img src="assets/branding/icon.png" alt="M3HT4 Logo" width="180">
</p>

<h2 align="center">Modern Hunting Terrain</h2>

<p align="center">
  <strong>Built for 3 Teams. Powered by 4 Pillars.</strong>
</p>

<p align="center">
  <em>Learn the data. Hunt the behavior. Plan the emulation. Improve together.</em>
</p>

<p align="center">

🔵 <strong>Blue Team</strong> &nbsp;&nbsp;•&nbsp;&nbsp;
🔴 <strong>Red Team</strong> &nbsp;&nbsp;•&nbsp;&nbsp;
🟣 <strong>Purple Team</strong>

<br><br>

🔎 <strong>Hunt</strong> &nbsp;&nbsp;•&nbsp;&nbsp;
🛡️ <strong>Detect</strong> &nbsp;&nbsp;•&nbsp;&nbsp;
♟️ <strong>Emulate</strong> &nbsp;&nbsp;•&nbsp;&nbsp;
📘 <strong>Train</strong>

</p>

---

<p align="center">
Made with ❤️ for the cybersecurity community.
</p>

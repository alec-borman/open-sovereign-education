# IEEE P3820/OS: The Open Standard for Sovereign, Culturally-Adaptive Education

[![IEEE SA](https://img.shields.io/badge/IEEE-P3820%2FOS-blue)](https://standards.ieee.org)
[![License: AGPL v3](https://img.shields.io/badge/Kernel-AGPLv3-green)](https://www.gnu.org/licenses/agpl-3.0)
[![Status: Draft](https://img.shields.io/badge/Status-Review%20Draft-yellow)]()

**A Protocol-First Framework for Educational Sovereignty in an AI-Driven World**

---

## README: What Is This?

This repository contains the specification for **IEEE P3820/OS**, a proposed open standard for sovereign, culturally-adaptive education infrastructure.

We are **not** building a single global education platform. We are building the **TCP/IP of education**—a lightweight, trusted protocol that enables:

- **Nations** to own their student data and curriculum
- **Teachers** to use AI tools that answer to them, not to corporations
- **Students** to carry verifiable learning records across borders
- **Cultures** to define what learning means, in their own terms

This is a constitutional framework, not a product. The code belongs to the people. The data belongs to the students. The curriculum belongs to the culture. The governance belongs to the community.

---

## Table of Contents

- [Preamble: The Philosophy](#preamble-the-philosophy)
- [Part I: Architectural Principles](#part-i-architectural-principles)
  - [Principle 1: Protocol Core + Modular Pedagogy](#principle-1-protocol-core--modular-pedagogy)
  - [Principle 2: Data Sovereignty](#principle-2-data-sovereignty)
  - [Principle 3: Linguistic Parity](#principle-3-linguistic-parity)
  - [Principle 4: Offline-First & Edge AI](#principle-4-offline-first--edge-ai)
- [Part II: The Open Source Stack](#part-ii-the-open-source-stack)
- [Part III: National Adoption Pathway](#part-iii-national-adoption-pathway)
- [Part IV: Cultural Adaptation Examples](#part-iv-cultural-adaptation-examples)
- [Part V: The Global Commons](#part-v-the-global-commons)
- [Part VI: Economic Model](#part-vi-economic-model)
- [Part VII: Governance & Ethical Design](#part-vii-governance--ethical-design)
- [Annex A: Glossary](#annex-a-glossary)
- [Annex B: Resolution of Outstanding Issues](#annex-b-resolution-of-outstanding-issues)
- [Annex C: Project Governance & Contribution Guide](#annex-c-project-governance--contribution-guide)

---

## Preamble: The Philosophy

The closed, proprietary education models of the 20th century created **digital colonialism**—nations dependent on foreign platforms, curricula, and data extractors. As AI accelerates, this dependency becomes existential: whoever controls the model controls the mind.

IEEE P3820/OS inverts this paradigm. This is not merely an open-source project; it is a **constitutional framework** for educational sovereignty:

- **Code that belongs to the people** (GPLv3/AGPLv3 for kernel components)
- **Data that belongs to the students** (GDPR+ sovereignty requirements)
- **Curriculum that belongs to the culture** (modular, translatable, adaptable)
- **Governance that belongs to the community** (multi-stakeholder stewardship)

We embrace exponential AI progress while anchoring education in timeless values: sovereignty, equity, and human flourishing.

---

## Part I: Architectural Principles

### Principle 1: Protocol Core + Modular Pedagogy

The system is structured as a **minimal protocol core** (invariant data and identity logic) surrounded by **modular learning logics** (culturally-determined pedagogies) and **pluggable AI models**.

#### The Invariant Protocol Core (Non-Negotiable)

This is the **TCP/IP layer**—the minimal set of rules that enable interoperability:

| Component | Specification |
|-----------|---------------|
| **Identity** | Decentralized Identifiers (DIDs) v1.0 + Verifiable Credentials |
| **Event Data** | 1EdTech Caliper Analytics v1.2 (profile: P3820/OS) |
| **Competency Framework** | CASE (Competencies and Academic Standards Exchange) v2.0 |
| **Interoperability** | LTI 1.3, OneRoster 1.1 |
| **Privacy** | IEEE 7000-2021 ethical design patterns |
| **Encryption** | AES-256 at rest, TLS 1.3 in transit |
| **Data Sovereignty** | Geolocation tagging + residency enforcement |

The core contains **no pedagogical assumptions**. It does not require mastery-based progression, age cohorts, or any specific learning theory. It simply defines how learning events, competencies, and identities can be represented and exchanged.

#### Modular Learning Logics (MLLs) — Optional, Pluggable

Nations or communities may implement one or more MLLs that encode pedagogical approaches. These are **reference implementations**, not requirements:

| MLL Type | Description | Reference Implementation Status |
|----------|-------------|--------------------------------|
| **Mastery-Based** | Progression logic requiring demonstrated competency | [./mll/mastery/](./mll/mastery) |
| **Apprenticeship** | Observation-based skill verification by mentors | [./mll/apprenticeship/](./mll/apprenticeship) |
| **Phenomenon-Based** | Cross-disciplinary project tracking | [./mll/phenomenon/](./mll/phenomenon) |
| **Oral Tradition** | Narrative assessment with speech-to-text | [./mll/oral/](./mll/oral) |
| *Future MLLs* | Community-contributed pedagogies | [Contribution Guide](./CONTRIBUTING.md) |

Each MLL is independently governed and versioned. The protocol core remains neutral.

#### The AI Layer (Pluggable, Locally Certified)

- **Model Registry:** Local/regional bodies certify models for use in their jurisdiction
- **Knowledge Tracing:** Multiple algorithms (Bayesian, deep, attentive) coexist
- **Inference:** ONNX, Llama.cpp, future neuromorphic backends
- **Transparency Reports:** Mandatory disclosure of training data, bias audits, performance metrics

---

### Principle 2: Data Sovereignty and Decentralized Identity

Every implementation must include a sovereign data layer to prevent centralized tracking:

| Requirement | Technical Implementation |
|-------------|--------------------------|
| **Data Residency** | Localized storage within national borders via regional clusters |
| **Decentralized Identity** | DIDs decouple student identity from centralized registries |
| **Data Portability** | Export in JSON-LD and CASE formats |
| **Algorithmic Transparency** | Mandatory disclosure of model logic for fairness audits |
| **Personal Data Vaults** | Optional Solid Pod integration for student-controlled storage |

---

### Principle 3: Linguistic Parity

Translation is a first-class architectural component. All core protocol messages are language-agnostic, relying on structured data rather than English templates.

- UI/UX localization via Unicode (RTL/LTR support)
- AI prompts use structured JSON-LD, not natural language
- Community translation workflows for curriculum modules

---

### Principle 4: Offline-First and Edge AI

Global adoption requires functionality where internet is intermittent:

| Capability | 2026 Target | 2030 Projection |
|------------|-------------|-----------------|
| **Local Inference** | Raspberry Pi 5: 10-18 tokens/sec (1B-3.8B quantized) | 50-100 tokens/sec |
| **Quantization** | INT8, GGUF Q4_0 | Neuromorphic compression |
| **Sync** | Peer-to-peer mesh networking | Satellite backhaul integration |
| **Power** | Solar + battery optimization | Ultra-low-power edge chips |

---

## Part II: The Open Source Stack

```
ieee-p3820/
├── protocol-core/                 # Invariant layer (AGPLv3)
│   ├── identity/                  # DID resolution, verification
│   ├── caliper/                   # Event schema validation
│   ├── case/                      # Competency framework parser
│   └── sovereignty/               # Geolocation, encryption
├── mll/                           # Modular Learning Logics (Apache 2.0)
│   ├── mastery/                   # Reference: Mastery-based progression
│   ├── apprenticeship/            # Reference: Mentor verification
│   ├── phenomenon/                # Reference: Project-based learning
│   └── oral/                       # Reference: Narrative assessment
├── ai-layer/                       # Pluggable AI (Apache 2.0)
│   ├── model-registry/            # Local certification tools
│   ├── kt-adapters/               # BKT, DKT, SAKT wrappers
│   ├── personalization/           # Recommendation engine
│   └── inference/                 # ONNX, Llama.cpp runtimes
├── lms-core/                       # Reference LMS (Apache 2.0)
│   ├── api/                       # LTI 1.3, OneRoster
│   ├── auth/                      # OAuth2, OpenID Connect
│   └── sync/                       # Offline-first mesh sync
├── content-framework/              # Authoring tools (MIT)
│   ├── compiler/                   # YAML/JSON-LD → CASE
│   ├── translator/                 # Community translation
│   └── exchange/                   # GUID-based curriculum sharing
├── interfaces/                      # Reference front-ends (MIT)
│   ├── student/                    # React Native/Flutter
│   ├── teacher/                     # Caliper dashboard
│   └── parent/                      # SMS/USSD gateway
└── security-core/                   # Governance tools (GPLv3)
    ├── audit/                       # Immutable event logs
    └── bias-tools/                   # Fairness audit suites
```

---

## Part III: National Adoption Pathway

### Phase 0: Readiness Assessment (3–6 Months)
- **Infrastructure:** Analyze device access, power reliability
- **Human Capital:** Evaluate teacher digital literacy, developer availability
- **Legal:** Gap analysis against ISO/IEC 23894, local data laws

### Phase 1: Protocol Implementation (12–18 Months)
- **Core Deployment:** Install protocol-core on national infrastructure
- **Identity Layer:** Integrate national ID with DIDs
- **Localization:** Translate UI, adapt initial curriculum modules
- **MLL Selection:** Choose and configure pedagogical modules

### Phase 2: Scale and Sustainability (24–36 Months)
- **Regional Rollout:** Deploy edge hardware with certified AI models
- **Teacher Training:** Budget for transformation (5× software cost)
- **Community Model Challenges:** Incentivize local AI development

### Phase 3: Continuous Evolution (Ongoing)
- **Benchmarking:** Annual evaluation of AI model performance
- **MLL Contributions:** Submit new pedagogical modules to commons
- **Ethical Audits:** Recurring bias and fairness reviews

---

## Part IV: Cultural Adaptation Examples

### Example 1: Kenya — Oral Tradition and Mobile Integration
- **Protocol Implementation:** Voice-first interfaces, SMS parent alerts
- **MLL:** Oral Tradition module with speech-to-text assessment
- **AI Certification:** Local models trained on Swahili/English narratives
- **Hardware:** Solar-powered Raspberry Pi clusters, feature phone gateway

### Example 2: Finland — Collaborative Mastery
- **Protocol Implementation:** Group Caliper events, verifiable credentials
- **MLL:** Phenomenon-Based + Mastery hybrid
- **AI Certification:** Explainability-focused models, teacher-in-the-loop
- **Hardware:** Recycled corporate laptops, community servers

### Example 3: Brazil — Indigenous Language Sovereignty
- **Protocol Implementation:** 180+ language packs, community mesh networks
- **MLL:** Oral Tradition + Apprenticeship modules
- **AI Certification:** Co-developed with tribes using IEEE 7000 value elicitation
- **Hardware:** Community-owned edge nodes, satellite backhaul

---

## Part V: The Global Commons

### The CASE Curriculum Exchange
Nations share content through the CASE network:

- **GUIDs:** Every learning objective receives a globally unique identifier
- **Forking:** Nations may adapt shared curricula to local needs
- **Alignment:** Automated mapping between competency frameworks

### The Hardware Independence Layer
P3820/OS remains hardware-agnostic with reference tiers:

| Tier | 2026 Hardware | Students per Device |
|------|---------------|---------------------|
| 1 | Raspberry Pi 5 + solar | 1–2 |
| 2 | Recycled corporate (x86/ARM) | 1 |
| 3 | Community servers + thin clients | 30–50 |

---

## Part VI: Economic Model

### Two-Layer Funding

**1. Upstream Maintenance Fund** (global, shared)
Maintains protocol-core, reference MLLs, security audits.

| GDP Tier (Per Capita) | Annual Contribution per Student |
|-----------------------|--------------------------------|
| Low (<$2,000) | $0.00 – $0.20 |
| Lower-Middle ($2k–5k) | $0.40 – $1.00 |
| Upper-Middle ($5k–15k) | $1.20 – $3.00 |
| High (>$15k) | $3.20 – $10.00 |

**2. Transformation Budget** (national, local)
Funds teacher training, hardware, localization, curriculum development.
*Expected ratio: 5× upstream contribution.*

**Sustainability Principle:** No donor or corporate sponsor gains algorithmic influence. Governance remains under multi-stakeholder control.

---

## Part VII: Governance & Ethical Design

### Two-House Governance Model

**Technical Steering Group (TSG)**
- Composition: Implementers, engineers, protocol experts
- Decision rule: IETF-style rough consensus
- Scope: Protocol-core changes, technical standards

**Stewardship Council**
- Composition: Teacher unions, Indigenous forums, Civil Society (UNESCO, etc.), National implementers, Student councils
- Decision rule: Supermajority vote for budget, ethical framework, dispute resolution
- Scope: Funding allocation, ethical audits, certification standards

### Ethical Value Requirements (EVRs)

Following IEEE 7000, abstract values translate into enforceable requirements:

| Value | EVR |
|-------|-----|
| **Transparency** | AI must provide human-understandable explanations for all recommendations |
| **Accountability** | Licensed professionals retain responsibility for high-stakes decisions |
| **Wellbeing** | System must track affect metrics and intervene to reduce stress |
| **Non-Domination** | No AI model may be mandated; teachers may override all recommendations |

---

## Annex A: Glossary

| Term | Definition |
|------|------------|
| **Protocol Core** | The invariant layer defining identity, events, competencies, and sovereignty |
| **MLL (Modular Learning Logic)** | A pluggable pedagogical module (e.g., mastery-based, apprenticeship) |
| **DID** | Decentralized Identifier (W3C standard) |
| **CASE** | Competencies and Academic Standards Exchange (1EdTech) |
| **Caliper** | Learning event analytics standard (1EdTech) |
| **Model Registry** | Local/regional body certifying AI models for deployment |

---

## Annex B: Resolution of Outstanding Issues

This section documents how the community has addressed concerns raised during the review process.

### Issue #1: "The Governance Mirage" — Who Really Decides?

**Resolution:** Adopted **Two-House Governance Model** (Annex C). Technical decisions are made by implementers via rough consensus; political/funding decisions by a representative council with supermajority rules. This separates technical evolution from political capture.

### Issue #2: "The Invariant Kernel is Not Neutral" — Pedagogical Colonialism

**Resolution:** The kernel is now a **pure protocol** with zero pedagogical assumptions (Part I, Principle 1). All learning logics are moved to **Modular Learning Logics (MLLs)** , which are optional, community-governed, and versioned independently. The protocol merely carries data; it does not prescribe how to interpret it.

### Issue #3: "Who Certifies AI Models?" — Single Point of Political Failure

**Resolution:** Certification is **decentralized to local/regional accredited bodies** (Part I, AI Layer). A model certified in Finland is valid in Finland; a model certified by a Brazilian indigenous council is valid in that context. The protocol defines the *format* of transparency reports, not the *content* of approval.

### Issue #4: "The Economic Model is Unsustainable" — Free Riders and Forks

**Resolution:** Separated funding into **Upstream Maintenance** (global, shared) and **Transformation** (national, local) (Part VI). Upstream contributions are tiered by GDP. The protocol's network effect (interoperability, shared MLLs, global student mobility) provides incentive to stay aligned rather than fork. Forks remain possible but lose access to the commons.

### Issue #5: "Teacher Resistance" — Surveillance vs. Empowerment

**Resolution:** Embedded teacher protections in protocol design:
- Default data sharing is *with teacher, not administrator*
- Ethical Value Requirements mandate explainability and override rights
- Teacher unions have permanent seats on Stewardship Council
- Reference MLLs include "teacher-in-the-loop" patterns

### Issue #6: "The Monolithic Failure Risk" — Cathedral vs. Bazaar

**Resolution:** Explicit pivot to **protocol-first architecture** (Preamble). The goal is not to build a single global platform but a *neutral substrate* that enables a diverse ecosystem of sovereign implementations. The TCP/IP analogy is now operationalized throughout.

---

## Annex C: Project Governance & Contribution Guide

### How We Make Decisions

**Technical Steering Group (TSG)**
- Meets monthly, open to all contributors
- Decisions by rough consensus (modeled on IETF)
- Focus: protocol-core changes, MLL reference implementations, security

**Stewardship Council**
- Meets quarterly, seats allocated per GDP tier + civil society
- Decisions by 2/3 supermajority
- Focus: budget approval, ethical framework updates, dispute resolution

### How to Contribute

We welcome contributions in several forms:

| Area | Where to Start | License |
|------|----------------|---------|
| **Protocol Core** | [./protocol-core/CONTRIBUTING.md](./protocol-core/CONTRIBUTING.md) | AGPLv3 |
| **MLL Reference Implementations** | [./mll/CONTRIBUTING.md](./mll/CONTRIBUTING.md) | Apache 2.0 |
| **AI Adapters** | [./ai-layer/CONTRIBUTING.md](./ai-layer/CONTRIBUTING.md) | Apache 2.0 |
| **Localization** | [./content-framework/translator/](./content-framework/translator/) | MIT |
| **Documentation** | [./docs/](./docs/) | CC-BY |

**First-time contributor?** Look for issues labeled `good-first-issue` or join our community calls (link in [README](./README.md)).

### Code of Conduct

All participants agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md), which prioritizes respectful, inclusive, and constructive collaboration.

---

## License & Copyright

- **Protocol Core:** AGPLv3 (ensures improvements remain open)
- **Reference Implementations (MLLs, LMS):** Apache 2.0 (maximizes adoption)
- **Documentation:** CC-BY 4.0

Copyright © 2026 IEEE P3820/OS Working Group. Contributors retain copyright over their contributions; the standard itself is open for implementation by anyone.

---

*"Education is the most powerful weapon which you can use to change the world." — Nelson Mandela*

*Let us ensure that weapon belongs to the people, not to the platforms.*

**[Star this repo](https://github.com/ieee-p3820/os)** • **[Join the mailing list](https://lists.ieee-p3820.org)** • **[Read the FAQ](./FAQ.md)**

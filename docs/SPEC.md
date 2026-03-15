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
  - [6.1 Upstream Maintenance Fund](#61-upstream-maintenance-fund)
  - [6.2 Transformation Budget](#62-transformation-budget)
  - [6.3 Proof of Contribution Mechanism](#63-proof-of-contribution-mechanism)
  - [6.4 Sustainability Principle](#64-sustainability-principle)
- [Part VII: Governance & Ethical Design](#part-vii-governance--ethical-design)
  - [7.1 Multi-Stakeholder Stewardship](#71-multi-stakeholder-stewardship)
  - [7.2 Two-House Governance Model](#72-two-house-governance-model)
  - [7.3 Ethical Value Requirements](#73-ethical-value-requirements)
  - [7.4 The Trust Layer – Solving the Oracle Problem](#74-the-trust-layer--solving-the-oracle-problem)
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
│   └── oral/                      # Reference: Narrative assessment
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
│   ├── teacher/                    # Caliper dashboard
│   └── parent/                     # SMS/USSD gateway
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

### 6.1 Upstream Maintenance Fund (Global, Shared)
Maintains protocol-core, reference MLLs, security audits, and trust infrastructure.

| GDP Tier (Per Capita) | Base Annual Contribution per Student | Maximum Discount (via Credits) | Effective Minimum |
|-----------------------|--------------------------------------|-------------------------------|-------------------|
| Low (<$2,000) | $0.00 – $0.20 | N/A (floor) | $0.00 |
| Lower-Middle ($2k–5k) | $0.40 – $1.00 | 25% | $0.30 – $0.75 |
| Upper-Middle ($5k–15k) | $1.20 – $3.00 | 50% | $0.60 – $1.50 |
| High (>$15k) | $3.20 – $10.00 | 75% | $0.80 – $2.50 |

### 6.2 Transformation Budget (National, Local)
Funds teacher training, hardware, localization, curriculum development.  
*Expected ratio: 5× upstream contribution (after discounts).*

### 6.3 Proof of Contribution Mechanism

#### 6.3.1 Contribution Types and Credit Values

| Contribution Type | Base Credits | Multipliers |
|-------------------|---------------|-------------|
| **Curriculum Module** (per 100 CASE objectives) | 10 | +2× if high adoption; +3× if multilingual |
| **Translation Pack** (per language, 90%+ coverage) | 15 | +2× for indigenous/low-resource languages |
| **MLL Reference Implementation** | 50 | +2× if includes teacher-in-the-loop patterns |
| **Certified AI Model** (with transparency report) | 30 | +2× if outperforms baseline on fairness metrics |
| **Teacher Training OER** (per module) | 5 | +2× if evidence of effectiveness |
| **Critical Security Audit** | 25–100 | Severity-based |
| **Peer Review of Contributions** (per review) | 1–5 | Based on complexity and turnaround time |

#### 6.3.2 Escrow and Impact Scoring
To prevent low-quality or AI-generated contributions from flooding the system:

- All contributions enter a **3-month escrow period** before credits are fully released.
- During escrow, contributions accumulate an **Impact Score** based on:
  - Number of downloads or adoptions (verified via telemetry with privacy safeguards)
  - Community ratings (on a 1–5 scale)
  - Quality audits by randomly selected peer reviewers
- Credits are released proportionally to the Impact Score (e.g., 80% score = 80% of base credits).
- Contributions failing to reach a minimum impact threshold after 6 months receive no credits and may be archived.

#### 6.3.3 Decentralized Peer Review
To avoid bottleneck at the Technical Steering Group, peer review is itself incentivized:

- Any contributor with a history of quality contributions may become a **reviewer** after completing a training module.
- Reviews are assigned via a **decentralized rotation algorithm** that prevents conflicts of interest.
- Reviewers earn **Peer Review Credits** (1–5 per review) which count toward the same discount and access benefits.
- Review quality is monitored: consistently poor reviews (determined by appeal and cross-review) result in reviewer suspension.

#### 6.3.4 Credit Decay and Expiration
- Credits expire **5 years** after issuance to encourage ongoing contribution and prevent legacy dominance.
- Unused credits simply vanish; no automatic renewal.

#### 6.3.5 Credit Redemption Options
- **Discounts on Upstream Contributions** (as per table in 6.1)
- **Enhanced Commons Access:**
  - Priority Curriculum Alignment Requests (10 credits)
  - Automated Translation Assistance (25 credits per language)
  - Dedicated Technical Integration Support (50 credits per engagement)
- **Technical Working Group Participation** (observer status): 100 credits per year

#### 6.3.6 Governance Protections
- Credits do **not** affect governance voting weight (preserves one-nation-one-vote principle in Stewardship Council).
- Credit caps: No single nation may earn more than **50%** of total annual credits, preventing dominance.
- All credit grants and redemptions are logged in a public, immutable transparency log.

### 6.4 Sustainability Principle
No donor or corporate sponsor gains algorithmic influence. Governance remains under multi-stakeholder control. The Contribution Credit system aligns self-interest with collective good, creating a **virtuous cycle**: contributions reduce costs while improving the commons for all.

---

## Part VII: Governance & Ethical Design

### 7.1 Multi-Stakeholder Stewardship
Governance is decentralized across six councils: Technical Steering, National Implementers, Civil Society (e.g., UNESCO), Teacher Unions, Student Councils, and Indigenous Forums.

### 7.2 Two-House Governance Model

**Technical Steering Group (TSG)**
- Composition: Implementers, engineers, protocol experts
- Decision rule: IETF-style rough consensus
- Scope: Protocol-core changes, technical standards, review of technical contributions

**Stewardship Council**
- Composition: Teacher unions, Indigenous forums, Civil Society (UNESCO, etc.), National implementers, Student councils
- Decision rule: Supermajority vote for budget, ethical framework, dispute resolution, and high-level policy
- Scope: Funding allocation, ethical audits, certification standards, amendments to contribution mechanisms

### 7.3 Ethical Value Requirements (EVRs)

Following IEEE 7000, abstract values translate into enforceable requirements:

| Value | EVR |
|-------|-----|
| **Transparency** | AI must provide human-understandable explanations for all recommendations |
| **Accountability** | Licensed professionals retain responsibility for high-stakes decisions |
| **Wellbeing** | System must track affect metrics and intervene to reduce stress |
| **Non-Domination** | No AI model may be mandated; teachers may override all recommendations |

### 7.4 The Trust Layer – Solving the Oracle Problem

Decentralized identity without a trust framework is just cryptography without confidence. P3820/OS addresses the "who verifies the verifiers" problem through a **layered attestation model** that does not require a centralized registrar.

#### 7.4.1 Trust Establishment Through Transparency, Not Authority

The protocol rejects the notion of a single root of trust. Instead, it establishes trust through **verifiable metadata about issuers**, enabling relying parties (universities, employers, other nations) to make their own trust decisions based on transparent criteria.

| Layer | Mechanism | Trust Basis |
|-------|-----------|-------------|
| **1. Issuer Self-Declaration** | DID Document includes `assertionMethod` and `service` endpoints with published accreditation claims | Transparency; anyone can inspect claims |
| **2. Attestation by Known Entities** | Existing trusted institutions (ministries, universities) issue Verifiable Credentials *about* issuers | Delegated trust; transitive |
| **3. Transparency Logs** | All issuer metadata and credentials anchored to public append-only logs (e.g., blockchain or Certificate Transparency-style logs) | Auditability; detection of fraud |
| **4. Reputation Networks** | Accumulated verification outcomes shared via trusted data exchange protocols | Statistical trust; community validation |

#### 7.4.2 The Issuer Accreditation Credential (IAC)

Any entity may issue an **Issuer Accreditation Credential** to another entity. This credential asserts that the issuer meets certain standards (e.g., "accredited by the Kenyan Ministry of Education to issue Secondary School credentials"). The IAC itself is a Verifiable Credential, creating chains of attestation.

**Example Trust Chain:**
```
University of Tokyo (trust anchor) 
    └─ accredits → Japanese Ministry of Education (IAC)
        └─ accredits → Kenya Ministry of Education (IAC)
            └─ accredits → Turkana Regional Education Council (IAC)
                └─ issues → "Advanced Calculus" credential to student
```

The University of Tokyo need not trust the Turkana Council directly. It trusts its own ministry, which trusts Kenya's ministry, which trusts the regional council. The chain is fully verifiable via DID resolution.

#### 7.4.3 Trust Registries (Optional, Jurisdiction-Specific)

Nations or consortiums may maintain **trust registries**—lists of approved issuers for specific purposes. These are **not global** but local to jurisdictions. A Japanese university may maintain a registry of foreign education ministries it recognizes. A Brazilian indigenous council may maintain a registry of community elders authorized to issue apprenticeship credentials.

The protocol defines a standard format for trust registries (JSON-LD with DID references) but does not mandate their existence or content.

#### 7.4.4 The "Advanced Calculus" Problem Solved

A university in Tokyo evaluating a credential from a remote Kenyan council would:

1. Resolve the credential's issuer DID to obtain its DID Document and any attached IACs.
2. Follow the chain of IACs until reaching an issuer the university explicitly trusts (e.g., Japanese Ministry of Education).
3. Verify each signature along the chain.
4. Optionally check if the credential's competency claims (CASE GUIDs) align with the university's own curriculum mappings.

If the chain terminates at an unknown issuer, the university may:
- Reject the credential
- Accept it with probationary conditions
- Query community reputation networks for additional context

The protocol enables all options; it prescribes none.

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
| **IAC** | Issuer Accreditation Credential |
| **Impact Score** | A measure of a contribution's real-world adoption and quality |
| **Contribution Credit** | Non-transferable, expiring token earned for contributions to the commons |

---

## Annex B: Resolution of Outstanding Issues

This section documents how the community has addressed concerns raised during the review process.

### Issue #1: "The Governance Mirage" — Who Really Decides?

**Resolution:** Adopted **Two-House Governance Model** (Section 7.2). Technical decisions are made by implementers via rough consensus; political/funding decisions by a representative council with supermajority rules. This separates technical evolution from political capture.

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

### Issue #7: "The Oracle Problem" — Who Verifies the Verifiers?

**Resolution:** Implemented **Layered Attestation Model** (Section 7.4). Trust is established through verifiable chains of Issuer Accreditation Credentials, not a centralized registrar. Relying parties (universities, employers) make their own trust decisions based on transparent issuer metadata and optional jurisdiction-specific trust registries. The protocol provides the cryptographic and data format infrastructure; it does not prescribe a single root of trust.

### Issue #8: "The Incentive Gap" — Why Contribute to the Commons?

**Resolution:** Implemented **Proof of Contribution mechanism** with escrow, impact scoring, and decentralized peer review (Section 6.3). Nations and organizations earn Contribution Credits for validated contributions. Credits redeem for discounts on upstream financial obligations and enhanced access to commons services. This creates a virtuous cycle where contribution reduces cost while improving the commons for all. Governance weight remains tied to GDP tier, preventing "buying influence."

### Issue #9: "Reviewer Bottleneck" — Scaling Peer Review

**Resolution:** Introduced **decentralized peer review** with reviewer incentives (Section 6.3.3). Any qualified contributor can become a reviewer, earning credits for reviews. A rotation algorithm ensures fair distribution and prevents conflicts of interest.

### Issue #10: "Credit Inflation" — Low-Quality Contributions

**Resolution:** Implemented **escrow and Impact Score** (Section 6.3.2). Credits are released only after a contribution demonstrates real-world adoption and quality, verified through usage telemetry, community ratings, and audits. Low-impact contributions receive reduced or zero credits.

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
- Focus: budget approval, ethical framework updates, dispute resolution, amendments to contribution parameters

### How to Contribute

We welcome contributions in several forms:

| Area | Where to Start | License |
|------|----------------|---------|
| **Protocol Core** | [./protocol-core/CONTRIBUTING.md](./protocol-core/CONTRIBUTING.md) | AGPLv3 |
| **MLL Reference Implementations** | [./mll/CONTRIBUTING.md](./mll/CONTRIBUTING.md) | Apache 2.0 |
| **AI Adapters** | [./ai-layer/CONTRIBUTING.md](./ai-layer/CONTRIBUTING.md) | Apache 2.0 |
| **Localization** | [./content-framework/translator/](./content-framework/translator/) | MIT |
| **Documentation** | [./docs/](./docs/) | CC-BY |
| **Peer Review** | Sign up via [reviewer onboarding](./REVIEWER.md) | N/A |

**First-time contributor?** Look for issues labeled `good-first-issue` or join our community calls (link in [README](./README.md)).

### Reviewer Onboarding
1. Complete the reviewer training module (available in `./REVIEWER_TRAINING.md`).
2. Submit three sample reviews of existing contributions.
3. Upon approval by a TSG member, receive reviewer status and begin earning credits.

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

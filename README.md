# SMEPro Intelligence Orchestration System (IOS+)

> **Stack:** OpenClaw Runtime (execution) → Interception/Proxy Layer → UDM + Compliance OS (deterministic policy) → Yellow Brick Road Pipeline (7-layer validation) → IOS+ consensus + 777-Handshake (approval) → cryptographically signed forensic audit package.

*For oil, gas, finance, healthcare, and government operators who need agentic AI that is defensible by design.*

---

## Patent Notice

**Patent 63/986,802** — Intelligence Orchestration System  
Additional patents pending under **SMEPro Intelligence Systems**  
All architecture, ontology, and pipeline definitions are **proprietary and confidential**.

---

## Overview

IOS+ is a compliance-first execution substrate for autonomous AI agents. It intercepts every intent, tool call, and system action before execution — routing each through deterministic policy, semantic decoding, and cryptographic audit — converting open-source agentic platforms like OpenClaw from high-risk experimental tools into production-grade, regulatory-defensible systems.

### The Problem

Modern agent platforms (OpenClaw, etc.) derive power from:
- **Local persistence** — survives reboots, runs continuously
- **Direct host access** — shell commands, file access, system APIs
- **Extensible plugin ecosystems** — community skills with unbounded capabilities

These same properties create attack surfaces that probabilistic safety cannot close:

| Threat | Vector | Impact |
|--------|--------|--------|
| ClawJacked | Gateway brute force → execution authority | Full host compromise |
| Supply-Chain | Malicious community plugins | Privileged code execution |
| Prompt Injection | Weaponized emails/documents | Unauthorized regulatory actions |

---

## Architecture

```
┌─────────────────────────────────────────────────────────────┐
│  Layer 4 — IOS+ Intelligence Orchestration System           │
│             [PATENT 63/986,802]                             │
│  Multi-agent consensus, human approval gateway, enforcement  │
├─────────────────────────────────────────────────────────────┤
│  Layer 3 — Yellow Brick Road Pipeline                       │
│  Signal → Semantic → Ontological → Regulatory →             │
│  Compliance → Operational → Forensics                       │
├─────────────────────────────────────────────────────────────┤
│  Layer 2 — Compliance OS + Universal Decoding Matrix (UDM)  │
│  Policy engine + semantic ontology                          │
│  Natural language intent → enforceable semantic tokens      │
├─────────────────────────────────────────────────────────────┤
│  Layer 1 — Interception Layer (High-Privilege Proxy)        │
│  All inbound RPC requests paused — no execution without     │
│  IOS+ authorization                                         │
├─────────────────────────────────────────────────────────────┤
│  Layer 0 — OpenClaw Gateway Runtime [MIT LICENSE]           │
│  Messaging, memory, tool execution, WebSocket control plane  │
└─────────────────────────────────────────────────────────────┘
```

**Critical property:** Layer 1 intercepts all execution before it reaches Layer 0. This is a **prevention system**, not a monitoring system.

---

## Repository Structure

```
smepro-ios/
│
├── core/                          # IOS+ Core — PATENTED
│   ├── ios-plus/                  # Intelligence Orchestration System
│   │   ├── interception-layer/    # High-privilege proxy
│   │   ├── consensus-engine/      # Multi-agent adjudication
│   │   ├── handshake-777/         # Human approval protocol
│   │   └── audit-trail/           # Cryptographic evidence packaging
│   ├── compliance-os/             # Policy engine
│   │   ├── policy-atoms/          # Machine-readable regulatory rules
│   │   ├── allow-deny-engine/     # Context-aware enforcement
│   │   └── policy-loader/         # Dynamic context-specific loading
│   ├── udm/                       # Universal Decoding Matrix
│   │   ├── ontology/              # Canonical semantic ontology
│   │   ├── decoders/              # NL → semantic token pipelines
│   │   └── dimensions/            # NAICS, SOC, jurisdiction, etc.
│   └── yellow-brick-road/         # 7-layer reasoning pipeline
│       ├── layer-1-signal/
│       ├── layer-2-semantic/
│       ├── layer-3-ontological/
│       ├── layer-4-regulatory/
│       ├── layer-5-compliance/
│       ├── layer-6-operational/
│       └── layer-7-forensics/
│
├── icoos/                         # Intelligence Compliance OS (ICOOS)
│   ├── core/                      # Shared compliance schema + form engine
│   ├── adapters/
│   │   ├── msogb/                 # Mississippi — REFERENCE IMPLEMENTATION
│   │   ├── rrc/                   # Texas — Phase 2
│   │   ├── ldnr/                  # Louisiana — Phase 2
│   │   ├── occ/                   # Oklahoma — Phase 3
│   │   ├── ndic/                  # North Dakota — Phase 3
│   │   └── nmocd/                 # New Mexico — Phase 3
│   └── cos-integration/           # COS ↔ skill dispatcher
│
├── docs/                          # Documentation
│   ├── whitepaper/                # Formal whitepaper
│   ├── security-disclosure/       # Coordinated disclosure package
│   ├── ciso-brief/                # O&G CISO executive brief
│   └── architecture/              # Diagrams and specs
│
├── skills/                        # OpenClaw skill manifests
│   ├── icoos-core.skill.yaml
│   ├── icoos-msogb.skill.yaml
│   └── ...
│
└── tests/                         # Test suites
    ├── injection-scenarios/       # Prompt injection test vectors
    ├── policy-validation/         # Compliance OS unit tests
    └── udm-resolution/            # UDM decoding accuracy tests
```

---

## Key Components

### Universal Decoding Matrix (UDM)

Converts ambiguous natural language intents into fully-specified, policy-evaluable semantic tokens.

**Example — O&G Monthly Filing:**
```
Input:  "file this month's production report for the Hartley lease"

Output: {
  NAICS:           "211120",              // Crude Petroleum Extraction
  jurisdiction:    "MS",                  // Mississippi
  regulatory_body: "MSOGB",
  form_id:         "MSOGB-Form-14",       // Monthly Production Report
  reporting_period:"2025-11",
  operator_id:     "OP-MS-00847",
  action_class:    "regulatory_submission",
  evidence_required: ["production_data", "operator_signature", "submission_receipt"],
  policy_atoms:    ["MSOGB.Rule.14.1", "MSOGB.Rule.14.2"]
}
```

### Yellow Brick Road Pipeline

Seven deterministic layers every action must pass before execution:

| Layer | Name | Function |
|-------|------|----------|
| 1 | Signal | Input sanitization, injection stripping |
| 2 | Semantic | NL intent classification |
| 3 | Ontological | UDM resolution → semantic token |
| 4 | Regulatory | Load applicable policy atoms |
| 5 | Compliance | Primary enforcement gate (ALLOW/BLOCK/ESCALATE) |
| 6 | Operational | Multi-agent consensus for ambiguous actions |
| 7 | Forensics | Cryptographic audit package signing |

### 777-Handshake Protocol

Three-step human-in-the-loop approval for `REQUIRE_APPROVAL` decisions:

1. **Notification** — IOS+ surfaces action + decoded token + escalation reason
2. **Contextual Review** — Operator reviews plain-language summary + policy atoms
3. **Explicit Approval** — Cryptographically authenticated APPROVE or DENY

Every approval is logged as a signed legal protection record.

---

## ICOOS State Adapters

| State | Agency | Adapter | Status | Key Forms |
|-------|--------|---------|--------|-----------|
| Mississippi | MSOGB | `icoos-msogb` | ✅ Phase 1 | Form-14, Form-2, Form-6, Form-P1 |
| Texas | RRC | `icoos-rrc` | 🔄 Phase 2 | W-2, W-3, P-5, PR |
| Louisiana | LDNR-OC | `icoos-ldnr` | 🔄 Phase 2 | Form-3, Form-1-A |
| Oklahoma | OCC | `icoos-occ` | 📋 Phase 3 | Form-1000, Form-1002A |
| North Dakota | NDIC | `icoos-ndic` | 📋 Phase 3 | OGD-003 |
| New Mexico | NMOCD | `icoos-nmocd` | 📋 Phase 3 | C-115, C-101, C-105 |

---

## Security Disclosure

Three documented attack vectors against open-source agentic platforms:

- **THREAT-01 ClawJacked** — Gateway brute force → execution authority
- **THREAT-02 Supply-Chain** — Malicious plugin code execution
- **THREAT-03 Prompt Injection** — Weaponized content → unauthorized actions

IOS+ mitigates all three deterministically. See [`docs/security-disclosure/`](docs/security-disclosure/) for coordinated disclosure package.

---

## Regulatory Context

IOS+ is purpose-built for deployment in environments governed by:

`MSOGB` · `RRC` · `LDNR` · `OCC` · `NDIC` · `NMOCD` · `BSEE` · `EPA` · `BLM` · `SOX` · `HIPAA` · `FISMA` · `FedRAMP`

---

## Contact & Collaboration

**Christopher Miguez**  
Founder — SMEPro Technologies / SMEPro Intelligence Systems  
📧 csmiguez@smepro.app

SMEPro invites coordinated technical review, standards collaboration, and joint deployment partnerships with model providers, platform operators, and regulatory bodies.

---

## License

**Proprietary — All Rights Reserved**  
Patent 63/986,802. Additional patents pending under SMEPro Intelligence Systems.  
The OpenClaw runtime dependency is MIT-licensed. All IOS+, Compliance OS, UDM, Yellow Brick Road, and ICOOS components are proprietary.

> *This repository is confidential. Distribution requires written consent of SMEPro Technologies.*

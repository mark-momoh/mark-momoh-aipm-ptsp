# Teamapt AIPM Reference Repo

This is the reference repository for the Teamapt AI-Powered Product Management (AIPM) onboarding process. It contains:

- **Six pre-defined capability anchors** — one per squad area
- **A worked example** — a complete Direct Debit subcapability, epic, and change spec
- **Blank templates** — copy these to start your own artifacts
- **Setup instructions** — see [SETUP.md](./SETUP.md)

---

## Who this is for

Teamapt Associate Product Managers completing the AIPM onboarding sequence. You will fork this repo to your personal GitHub account and use it as the base for your own artifacts.

---

## Repo structure

```
aipm-reference-repo/
├── README.md                   — This file
├── SETUP.md                    — Step-by-step onboarding guide
│
├── capabilities/               — Pre-defined capability anchors (Idris writes these)
│   ├── CAPABILITY-TAPT-DDBT.md — Direct Debit Operations
│   ├── CAPABILITY-TAPT-DISB.md — Disbursement Processing
│   ├── CAPABILITY-TAPT-COLL.md — Collections and Payments
│   ├── CAPABILITY-TAPT-PTSP.md — Terminal Service Provider Operations
│   ├── CAPABILITY-TAPT-TPPC.md — Third Party Processing
│   └── CAPABILITY-TAPT-TRXN.md — Transaction Processing Suite
│
├── subcapabilities/            — WORKED EXAMPLE: Direct Debit mandate management
│   └── SUBCAP-TAPT-DDBT-MAND.md
│
├── epics/                      — WORKED EXAMPLE: Mandate creation epic
│   └── EPIC-TAPT-DDBT-MAND-EP00001.md
│
├── release/                    — WORKED EXAMPLE: Change spec
│   └── change-spec.md
│
└── templates/                  — Blank templates — copy and rename these
    ├── subcapability-template.md
    ├── epic-template.md
    └── change-spec-template.md
```

---

## Important naming note

The `TAPT` platform code is **temporary** and signals pre-platformisation. When Teamapt migrates to the Moniepoint GitHub org, capability IDs will be reassigned by the Head of Platform. Your artifacts will be migrated — not discarded.

---

## Questions?

Slack Idris Aliyu (@ialiyu).

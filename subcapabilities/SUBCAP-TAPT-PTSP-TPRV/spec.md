---
id: SUBCAP-TAPT-PTSP-TPRV
name: Terminal Provisioning
capability: CAPABILITY-TAPT-PTSP
platform: TAPT
status: active
owner: Mark Momoh

personas:
  - operations-team
  - third-party-admin

channels:
  - POS
  - INTERNAL_SYSTEM

problem: |
  There is no digital path for back office admins to assign POS terminals to third-party
  admins (acquirers), or for third-party admins to assign those terminals to their
  merchants. The terminal provisioning flow — from inventory allocation to merchant-ready
  terminal — does not yet exist within the Aptpay PTSP platform, leaving assignment
  untracked and error-prone.

design_refs:
engineering_refs:
deprecation_reason:
---

## Description

Terminal Provisioning covers the end-to-end digital assignment of POS terminals from
the Aptpay PTSP inventory to merchants. A back office admin assigns a terminal from
virtual inventory (via the Moniepoint virtual inventory API) to a third-party admin
(acquirer). The third-party admin then assigns that terminal to one of their merchants
through the portal. The subcapability includes validation to prevent duplicate terminal
IDs and incorrect merchant-terminal mappings before a terminal goes live.

## Success Metrics

| Metric | Target |
|---|---|
| Time from terminal assignment request to merchant-ready | TBD |

## Scope Boundaries

**In scope:**
- Back office admin assignment of terminals from inventory to a third-party admin
- Third-party admin assignment of terminals to their merchants
- Integration with the Moniepoint virtual inventory API for terminal record retrieval
- Assignment validation — duplicate terminal ID checks and merchant mapping verification

**Out of scope:**
- Physical key injection
- SIM and connectivity setup
- Terminal repairs and maintenance
- Terminal decommissioning
- Agent onboarding (separate subcapability)

## Dependencies

- Moniepoint virtual inventory API — terminal records must exist in inventory before
  assignment can proceed; owned by the virtual inventory team
- Terminal Management System (TMS) — terminal configurations are anchored here
- CAPABILITY-TAPT-TRXN — transaction routing depends on the correct terminal-merchant
  mapping established by this subcapability

## Open Questions

- What is a realistic target for time from assignment request to merchant-ready? Is
  there an existing ops SLA we can use as a baseline for the TBD metric target?

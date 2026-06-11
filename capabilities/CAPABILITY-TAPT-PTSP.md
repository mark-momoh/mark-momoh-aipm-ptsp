# Capability: Terminal Service Provider Operations

```yaml
id: CAPABILITY-TAPT-PTSP
name: Terminal Service Provider Operations
platform: TAPT
status: active
owner: Head of Platform (Idris Aliyu — acting, pre-platformisation)

personas:
  - agent
  - merchant
  - operations-team
  - field-support
  - third-party-admin

channels:
  - POS
  - INTERNAL_SYSTEM

dependencies:
  - CAPABILITY-TAPT-TRXN  # Transaction Processing Suite
  - NIBSS (Nigeria Inter-Bank Settlement System)
  - CBN PTSP licensing framework
  - Terminal management system (TMS)

description: |
  Terminal Service Provider (PTSP) Operations covers the full lifecycle of POS terminal
  deployment, management, and transaction processing under the Teamapt PTSP licence.
  This includes terminal provisioning, agent onboarding, transaction routing, settlement,
  dispute management, and regulatory compliance reporting for all POS terminals under
  the Aptpay PTSP framework.

success_metrics:
  - Terminal uptime >= 98% across deployed estate
  - Transaction approval rate >= 95%
  - Agent onboarding cycle time <= 3 business days
  - Settlement accuracy rate 100%
  - Dispute resolution within regulatory SLA (5 business days)
```

---

## Subcapabilities under this capability

| Subcapability | Owner | Status |
|---|---|---|
| *(To be created by Mark Momoh)* | Mark Momoh | Pending |

---

## Notes

This capability is owned by the Aptpay PTSP squad. Mark Momoh (APM) is responsible for subcapabilities and epics under this capability.

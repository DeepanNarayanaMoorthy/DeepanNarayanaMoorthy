<div align="center">

# 🟢 Deepan Narayanamoorthy
### Status: All Systems Operational

</div>

---

## INCIDENT REPORT — INC-0001

**Title:** Engineer discovered running production infrastructure without supervision since 2023
**Severity:** SEV-3 (nobody is paging anyone, which is the point)
**Status:** `Resolved` — ongoing monitoring in place

### Summary
A Senior DevOps / Cloud Engineer was found at **[Everstage](https://www.everstage.com)**, quietly keeping a sales-performance-management platform's infrastructure from catching fire. Previously spotted at **Caterpillar Inc.**, where 30+ microservices across AWS and Azure somehow stayed standardized instead of diverging into 30+ different problems.

### Root Cause
Chronic inability to leave infrastructure undocumented, unautomated, or running on long-lived credentials. Known to open a terminal unprompted.

### Impact
- Release downtime cut by **3 hours** by catching broken ECS deploys before they became someone else's problem
- Long-lived AWS keys ripped out of CI/CD org-wide, replaced with **GitHub OIDC** — zero standing credentials left to leak
- Production incident rate down **20%** via auto-scaling that actually scales
- "Why does this cost this much" turned into an actual cost-attribution story, instead of a shrug

### Resolution
Terraform across prod / preprod / sandbox, reproducible by design, drift not welcome. Datadog + Atlassian Statuspage wired together so outages get a status page before they get a Slack thread. AWS Certified Solutions Architect — Associate, in case the badge matters more than the Terraform state file. (It doesn't.)

### Action Items
- [x] Stop storing secrets in places secrets shouldn't be
- [x] Make the pipeline fail *loudly* instead of quietly
- [ ] Convince everyone that "works on my machine" was never a valid root cause
- [ ] Take a vacation that doesn't involve checking PagerDuty

---

## boot.log

```
[  OK  ] Started aws.service (Solutions Architect — Associate)
[  OK  ] Started terraform.service (prod, preprod, sandbox — no drift)
[  OK  ] Started github-oidc.service (long-lived keys: deprecated)
[  OK  ] Started datadog.service + statuspage.service
[  OK  ] Started incident-rca.service (nginx, snowflake, vpc, queues)
[ WARN ] coffee.service restarting (exit code: EMPTY_MUG)
```

---

## Escalation Chain

| Priority | Channel |
|---|---|
| P1 — actually urgent | [Email](mailto:deepanntech@gmail.com) |
| P2 — professional curiosity | [LinkedIn](https://www.linkedin.com/in/deepann/) |
| P3 — "does this count as an incident" | [Resume](https://deepann.pages.dev/resume/) |
| P4 — just browsing | [Portfolio](https://deepann.pages.dev) |

<div align="center">

*99.9% uptime SLA. The 0.1% is where all the good stories are.*

</div>

# Deepan Narayanamoorthy

**Senior DevOps / Cloud Engineer** — AWS & Azure infrastructure, SRE practices, cost-aware architecture.

I own infrastructure end to end: Terraform across prod/preprod/sandbox without drift, CI/CD migrated off long-lived cloud keys onto GitHub OIDC, and the observability + incident-response work that keeps production honest. AWS Certified Solutions Architect — Associate.

Currently at **[Everstage](https://www.everstage.com)**, building and securing the infra behind a sales-performance-management platform. Previously at **Caterpillar Inc.**, standardizing cloud infra for 30+ microservices across AWS and Azure.

```
$ curl -s https://deepann.pages.dev/api/whoami | jq

{
  "role": "Senior DevOps / Cloud Engineer",
  "cloud": ["AWS", "Azure"],
  "cert": "AWS Solutions Architect — Associate",
  "stack": ["Terraform", "GitHub Actions", "Docker", "Datadog"],
  "currently": "Everstage",
  "previously": "Caterpillar Inc."
}
```

**What I focus on**

- Infrastructure as code (Terraform, CloudFormation, ARM) that stays reproducible across every environment, not just the one it was written for
- Eliminating long-lived cloud credentials — GitHub OIDC / short-lived auth across CI/CD, org-wide
- Observability and incident response: Datadog monitors/alerts tied to a public status page, so outages get caught before they get reported
- Cross-system RCA for failures without an obvious root cause — nginx, Snowflake, VPC, message queues
- Turning "nobody knows why this costs this much" into an actual cost-attribution and rightsizing story

---

[Resume](https://deepann.pages.dev/resume/) · [Portfolio](https://deepann.pages.dev) · [LinkedIn](https://www.linkedin.com/in/deepann/) · [Email](mailto:deepanntech@gmail.com)

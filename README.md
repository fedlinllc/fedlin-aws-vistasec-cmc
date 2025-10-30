# FEDLIN — AWS VistaSec CMC (Continuous Monitoring Center)

**Brand:** Security Architecture · Vulnerability Management · Compliance Automation  
**Delivery stance:** GitHub Actions (OIDC-only) · Evidence stays in the customer AWS account

This is the **public brief** for Fedlin’s AWS continuous monitoring service. It is the public-facing version of our earlier `fedlin-aws-monitoring` work.

## What this service does
- Aggregates AWS security signals (CloudTrail, Config, GuardDuty, Security Hub) into an audit-friendly view
- Maps those signals to SOC 2 / ISO 27001 / HIPAA-style questions
- Leaves evidence in **your** AWS account (S3/logs), not in this repo
- Uses GitHub Actions with **OIDC** so there are **no long-lived AWS keys**

## Who it’s for
- SMBs / healthcare / regulated teams that must *show* AWS security posture
- MSPs that want a repeatable monitoring story
- Customers that already have an AWS security baseline

## What’s in this repo
- `SERVICE_SCOPE.md` — what VistaSec CMC watches
- `EVIDENCE_MODEL.md` — where to keep proof in your AWS
- `DELIVERY_MODEL.md` — how we deliver it via OIDC
- `.github/workflows/` — example OIDC-only workflow
- `SECURITY.md` — how to report issues

## What’s **not** in this repo
- Account IDs, ARNs, or real exports
- Customer screenshots
- Full internal runbooks

---

Need this implemented in your AWS account?

📬 info@fedlin.com  
🌐 https://www.fedlin.com

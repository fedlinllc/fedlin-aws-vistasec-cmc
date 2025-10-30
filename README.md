# FEDLIN – AWS VistaSec / Central Monitoring & Compliance (CMC)

**Security Solutions Architecture · Vulnerability Management · Compliance Automation**

A customer-tenant-first monitoring and compliance view for AWS environments that need ongoing visibility, alerting, and audit-friendly evidence — without moving logs or secrets into FEDLIN-controlled infrastructure. This service is the public description; deployment assets are private.

---

## Who this is for

- Security teams that want CloudWatch/Security Hub surfaced in a consistent way
- MSPs / MSSPs that need to monitor multiple customer AWS accounts/organizations
- Regulated or PHI-adjacent orgs that need SOC 2 / ISO 27001 style evidence
- Subcontract-ready engagements where the prime must keep the tenant’s data

---

## What it delivers

- Standardized AWS monitoring view (CloudWatch, Security Hub, Config signals)
- Optional dashboarding / alerting suitable for compliance reporting
- Hooks that can be paired with the **AWS Security Baseline** service
- GitHub Actions (OIDC-only) delivery patterns
- Clear separation between public description and private deployment automation

> **Public repo policy:** This repository describes the service and delivery pattern. It does **not** contain customer-specific values, account IDs, log group names, or Terraform state.

---

## Evidence model (customer-owned)

- Logs, metrics, and evidence stay in **the customer’s AWS account(s)**
- FEDLIN automates setup through **GitHub Actions with OIDC only**
- Customer can export evidence directly from their AWS-native services
- When subcontracting, the prime keeps ownership of the customer tenant

This aligns with SOC 2, ISO 27001, and HIPAA-style evidence expectations.

---

## Delivery method

- **Primary:** GitHub Actions with OIDC-only into AWS
- **IaC options:** Terraform / policy-as-code for monitoring assets
- **Scripting:** bash / python helpers
- **Engagement model:** Independent / C2C, subcontract-ready, MSP-friendly

---

## Deployment assets

Deployment assets (Terraform modules, monitoring configs, per-tenant params, workflow files) are kept in the **private** repository:

👉 **\`fedlin-aws-vistasec-cmc-deployment\`**

This public repo tracks the service description, not the customer code.

---

## Related services

- FEDLIN – AWS Security Baseline (\`fedlin-aws-security-baseline\`)
- FEDLIN – Microsoft 365 Security Baseline (\`fedlin-m365-security-baseline\`)
- FEDLIN – Google Workspace HIPAA Baseline (\`fedlin-gws-hipaa-baseline\`)
- FEDLIN – DMARC / SPF / DKIM (\`fedlin-dmarc-spf-dkim\`)

---

## About FEDLIN

**FEDLIN** delivers:  
**Security Solutions Architecture · Vulnerability Management · Compliance Automation**

Independent / C2C · Subcontract-ready · Customer-tenant-first

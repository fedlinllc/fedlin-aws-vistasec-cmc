# FEDLIN – AWS VistaSec / CMC

[![Terraform](https://img.shields.io/badge/IaC-Terraform-623CE4?logo=terraform)](https://www.terraform.io/)
[![AWS](https://img.shields.io/badge/Cloud-AWS_Serverless-FF9900?logo=amazon-aws)](https://aws.amazon.com/)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python)](https://www.python.org/)
[![ISO 27001](https://img.shields.io/badge/ISO%2027001-Mapped-1f77b4)](#compliance-coverage)
[![SOC 2](https://img.shields.io/badge/SOC%202-Mapped-d62728)](#compliance-coverage)
[![NIST 800-53](https://img.shields.io/badge/NIST%20800--53-Mapped-2ca02c)](#compliance-coverage)
[![Maintained](https://img.shields.io/badge/Maintained-Yes-green)](#)

**VistaSec** = **Vista**bility + **Sec**urity  
**CMC** = **C**ontinuous **M**onitoring & **C**ompliance

Multi-cloud security monitoring and compliance automation platform that helps organizations prepare for and maintain SOC 2, ISO 27001, HIPAA, and NIST compliance. Built on serverless AWS architecture with customer-retained evidence.

[📧 Contact](mailto:info@fedlin.com) · [📞 Book Consultation](https://calendar.app.google/7z8eAZPvrW82jtxk6) · [🌐 fedlin.com](https://www.fedlin.com)

---

## 🎯 What This Delivers

A serverless security platform that continuously monitors multi-cloud environments and automatically maps findings to regulatory frameworks.

**Designed for:**
- **Compliance teams** preparing for SOC 2, ISO 27001, HIPAA, or NIST assessments
- **Organizations** needing continuous security monitoring with audit-ready evidence
- **MSPs/MSSPs** managing security and compliance for multiple clients
- **Security teams** requiring centralized visibility across AWS, Azure, GCP, and SaaS platforms

**Key capabilities:**
- Automated security finding aggregation across cloud providers
- Compliance framework mapping (ISO 27001, SOC 2, NIST 800-53, HIPAA)
- Continuous evidence collection and retention
- CloudWatch dashboards and alerting
- Customer-retained data (no vendor lock-in)

---

## 🏗️ Platform Architecture

### Multi-Cloud Security Monitoring

VistaSec/CMC provides centralized visibility across:

| Environment | Monitoring Capabilities |
|-------------|------------------------|
| **AWS** | Security Hub findings, Config compliance, GuardDuty threats, IAM analysis, S3 exposure, EC2 security groups |
| **Azure** | Security Center recommendations, Secure Score tracking, Defender findings |
| **GCP** | Security Command Center findings, asset inventory, policy violations |
| **GitHub** | Dependabot vulnerabilities, secret scanning alerts, repository security |
| **GitLab** | Project vulnerabilities, dependency scanning results |
| **Notion** | User access auditing, public page detection, data exposure risks |
| **Infrastructure** | TLS certificate monitoring, endpoint health checks, availability tracking |

### Serverless Event-Driven Design
```
Scheduled Events (CloudWatch Events)
         ↓
Multi-Cloud Scanners (AWS Lambda)
         ↓
Centralized Storage (DynamoDB)
         ↓
Compliance Calculator (Lambda)
         ↓
Dashboards & Evidence Exports (CloudWatch + S3)
```

**Infrastructure Efficiency:**
- Runs on AWS Free Tier for typical monitoring workloads
- Production deployments typically cost $5-50/month in AWS infrastructure
- Serverless architecture scales automatically with findings volume
- No dedicated servers or ongoing maintenance overhead

---

## 📊 Compliance Framework Coverage

VistaSec/CMC automatically maps security findings to compliance controls:

**ISO 27001 Coverage:**
- A.9 (Access Control): IAM policies, MFA enforcement, privileged access
- A.12 (Operations Security): Logging, monitoring, change management
- A.13 (Communications Security): Network controls, encryption, segmentation
- A.14 (System Acquisition): Secure development, security in projects

**SOC 2 Trust Services:**
- CC6.1: Logical and physical access controls
- CC6.6: Restricts access to sensitive data  
- CC7.2: System monitoring
- CC7.4: Security incident detection and response

**NIST 800-53 (Rev 5):**
- AC Family: Access Control
- AU Family: Audit and Accountability
- CM Family: Configuration Management
- IA Family: Identification and Authentication
- SC Family: System and Communications Protection

**HIPAA Security Rule:**
- §164.308(a)(1)(ii)(D): Information system activity review
- §164.308(a)(5)(ii)(C): Log-in monitoring
- §164.312(b): Audit controls
- §164.312(c)(2): Mechanism to authenticate ePHI

---

## 🔒 Customer-Tenant-First Architecture

Unlike traditional SaaS monitoring platforms that require sending your security data to third-party systems:

**All evidence stays in your AWS account:**
- Security findings stored in your DynamoDB tables
- Logs retained in your S3 buckets with your encryption
- CloudWatch dashboards visible in your console
- Complete data sovereignty and control

**FEDLIN deployment approach:**
- Infrastructure deployed via Terraform in your AWS account
- GitHub Actions with OIDC (no long-lived credentials)
- One-time setup, customer maintains ongoing access
- Can be removed cleanly with no vendor dependencies

**Benefits for regulated environments:**
- Satisfies data residency requirements
- Simplifies vendor risk assessments
- Supports SOC 2 / ISO 27001 / HIPAA / NIST evidence expectations
- No ongoing data processing agreements beyond initial deployment

---

## 🎯 Use Cases

### SOC 2 Type II Audit Preparation

**Challenge:** Organization needs continuous monitoring evidence for SOC 2 audit  
**Solution:** VistaSec/CMC provides 90-day evidence trail with automatic control mapping  
**Outcome:** Passed audit with comprehensive monitoring evidence

### MSP Multi-Client Monitoring

**Challenge:** MSP managing security for 15+ client environments across AWS, Azure, GCP  
**Solution:** Customer-tenant-first model with per-client evidence isolation  
**Outcome:** Standardized security monitoring, audit-ready client reports

### Healthcare Organization HIPAA Compliance

**Challenge:** Multi-cloud environment needs HIPAA Security Rule monitoring  
**Solution:** Automated mapping to HIPAA controls with continuous evidence collection  
**Outcome:** Real-time visibility, compliance dashboard for stakeholders

---

## 🤝 Engagement Models

**Direct Deployment**  
Complete VistaSec/CMC setup in your AWS account with configuration and training.

**MSP Partnership**  
White-label deployment for monitoring your managed clients with aggregated reporting.

**Consulting Business Services**  
FEDLIN operates as an independent consulting firm, open to contract and C2C engagements for security architecture and compliance automation projects.

---

## 📞 Get Started

**Primary Contact:** [info@fedlin.com](mailto:info@fedlin.com)  
**Book Consultation:** [Google Calendar](https://calendar.app.google/7z8eAZPvrW82jtxk6) or [Arrangr](https://arrangr.com/fedlin)  
**Demo:** Available upon request  

### Related FEDLIN Services

- **[AWS Security Baseline](https://github.com/fedlinllc/fedlin-aws-security-baseline)** - Deploy security controls that VistaSec monitors
- **[M365 Security Baseline](https://github.com/fedlinllc/fedlin-m365-security-baseline)** - Microsoft 365 hardening
- **[Google Workspace HIPAA](https://github.com/fedlinllc/fedlin-gws-hipaa-baseline)** - GWS compliance configuration
- **[DMARC/SPF/DKIM](https://github.com/fedlinllc/fedlin-dmarc-spf-dkim)** - Email authentication

---

## 📋 Repository Note

This repository describes the VistaSec/CMC service and architecture approach. Deployment assets (Terraform modules, Lambda functions, configuration templates) are provided as part of paid engagements.

**FEDLIN LLC**  
Security Solutions Architecture · Vulnerability Management · Compliance Automation  
Independent · Contract/C2C · Customer-tenant-first

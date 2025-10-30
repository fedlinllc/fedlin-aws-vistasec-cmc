# Delivery Model — AWS VistaSec CMC

1. **Access prep** — customer creates an AWS role that trusts GitHub OIDC
2. **Baseline monitoring** — Fedlin runs/guides the monitoring checks
3. **Evidence capture** — evidence is stored in the **customer** AWS account
4. **Handoff** — customer/MSP receives scope + evidence model
5. **(Optional)** schedule CI runs in GitHub to keep posture current

# Evidence Model (Public-Safe)

| Area              | Evidence Source     | Lives in        | Notes                           |
|-------------------|---------------------|-----------------|---------------------------------|
| Logging           | CloudTrail config   | Customer AWS     | Proves audit logging enabled    |
| Resource tracking | AWS Config          | Customer AWS     | Proves resource visibility      |
| Threat detection  | GuardDuty / Sec Hub | Customer AWS     | Proves detection in place       |
| Deployments (CI)  | GitHub Actions run  | Customer GitHub  | Proves OIDC-only delivery       |

> FEDLIN does **not** store customer evidence in this public repo.

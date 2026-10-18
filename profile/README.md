# Niftrox

**The change-evidence ledger for Azure estates.**

Azure keeps the before and after of a change for 14 days and the operation for 90. Most postmortems and every audit happen later than that. Niftrox builds **ChangeOps**: a ledger of every change Azure records, across the control plane, Entra ID, Kubernetes, Key Vault and later SQL, with who made it and the property-level difference, kept for two years, sealed every day with an external timestamp, and served to engineers, to the customer's own AI assistants over MCP, and to auditors as tamper-evident evidence packs and a period report.

## What it is

- One record per change: when, where, what, who, the before and after, and a pointer back to Azure's own record. The same change seen in two Azure logs is one record, and actors stay named after the identity is gone.
- Sealed daily: each day's records hash into one root, chained to the day before and anchored with an RFC 3161 timestamp. A frozen evidence pack verifies offline, without an account.
- Read-only by construction: admin consent, the Reader role and federated workload identity. No credential is exchanged or held, nothing is installed in the customer's estate, and nothing is written to their cloud.
- MCP at the core: Claude, ChatGPT, GitHub Copilot, Copilot Studio and Azure SRE Agent connect with the customer's own login and roles, and every call is audited. ChangeOps runs no model of its own, so the same question returns the same answer.

## What it is not

Not a log platform, an APM, a SIEM, an alerting product or an incident manager. It reads raw log records to build one normalised record per change and keeps no copy of them outside frozen packs. It ranks nothing and summarises nothing; the customer's agent does the reasoning.

## Who it is for

Azure-first organisations of a few hundred to a few thousand staff with a platform, cloud or SRE team and an on-call rotation, in the UK and EU first. Two buyers: the platform lead who owns the estate and asks "what changed?" after an outage, and the security or compliance owner who needs proof of every production change, by whom, for SOC 2, ISO 27001, DORA and NIS2.

## Status

In build. Design partners connect in 2027; paid pilots follow in 2028. The founder manual and MVP specification are maintained as living documents and drive the build.

Reach out at [amir@niftrox.com](mailto:amir@niftrox.com) for design-partner or partnership conversations.

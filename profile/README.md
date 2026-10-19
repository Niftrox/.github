# Niftrox

**The change-evidence ledger for Azure estates.**

Azure forgets what a change did. The Activity Log keeps the operation and the caller for 90 days, and the before and after of a resource change only for 14. Postmortems and audits usually come later than that, and once an identity is deleted, its changes can no longer be tied to a name.

Niftrox builds **ChangeOps**, a ledger of every change Azure records across the control plane, Entra ID, Kubernetes and Key Vault: what changed, who changed it, and the before and after where the source records one. It keeps the record for up to two years, seals each day's entries with an external timestamp so nobody can quietly alter them, and serves it to engineers in a web app, to the customer's own AI assistants over MCP, and to auditors as tamper-evident evidence packs and a quarterly "every production change, by whom" report.

## What we are

A focused B2B platform for Azure-first companies. One record per change, actors named even after their identity is deleted, the same answer every time, and evidence a third party can check without asking us. ChangeOps runs no model of its own; the customer's assistants query the ledger through the MCP server.

## What we are not

Not a log platform, an APM, a metrics or tracing tool, a SIEM, an alerting product or an incident manager. ChangeOps is read-only: it never holds a customer credential and never changes a customer's cloud. It keeps one normalised record per change, not copies of raw logs.

## Who it is for

Established Azure-first companies of 200 to 5,000 staff, in the UK and EU first. Two people buy it: the platform or cloud lead, who needs memory for postmortems and "nobody changed anything" incidents, and the security and compliance owner, who needs change-control evidence for SOC 2, ISO 27001, DORA and NIS2. The users are on-call engineers, engineers writing postmortems weeks later, auditors sampling changes, and the organisation's AI agents.

## Status

Active build. Design-partner conversations are open for Azure-first teams that recognise the problem from their own postmortems or audits.

Reach out at [amir@niftrox.com](mailto:amir@niftrox.com) for pilot or partnership conversations.

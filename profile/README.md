# Niftrox

**Incident-time change evidence for Azure platform teams.**

Roughly seven in ten production outages trace back to a change in a live system. The painful gap during an incident is not lack of logs — every cloud generates plenty. The pain is the manual stitching: at 3am, correlating control-plane events, resource changes, and Kubernetes mutations across four or more separate Azure interfaces while the page is still firing.

Niftrox builds **ChangeOps**, a multi-tenant B2B platform that answers one narrow question during a live production incident: what changed in the window, who changed it, and which changes are most worth checking first. It packages Azure Activity Log, Resource Graph change history, and AKS audit into a ranked, scored evidence pack with honest confidence labels — turning twenty-to-forty minutes of portal-hopping into under five.

## What we are

A focused B2B platform built for Azure-heavy engineering teams that have felt the 3am investigation pain personally. We stay narrow on purpose: incident-time change correlation is one well-defined job, and the existing native tooling has real workflow gaps there. The differentiator is not raw log access — Azure already provides that free. It is the investigation workflow, the ranked evidence packaging, the honest confidence labels, the tenant-safe multi-org onboarding, and a normalised change schema that the hyperscalers cannot easily replicate without breaking their own product boundaries.

## What we are not

Not a SIEM. Not an APM platform. Not a log ingestion pipeline. Not an autonomous remediation tool. ChangeOps does not replace Datadog, New Relic, Splunk, or Azure Monitor — it sits alongside them and picks up the moment a responder asks "what just changed?"

## Who it is for

Platform and SRE teams running production workloads on Azure with several AKS clusters in flight. The buyer is typically a head of platform, an SRE manager, or an engineering director who has been paged at 3am and knows what forty minutes of manual log hunting costs the on-call rotation. Initial focus is the UK and Western Europe, with strongest pull from sectors where evidence packaging is independently valuable: fintech, insurtech, health tech, and B2B SaaS under live compliance pressure.

## Status

Active build. Engineering, infrastructure, and the product surface are being shipped through a sequence of small, audited slices. The product specification, founder manual, and architectural blueprint are maintained as living documents rather than one-off deliverables — they evolve as pilots inform the design. Design-partner conversations are open for Azure-first teams that recognise the problem from their own incident history.

Open an issue on this organization to start a conversation about pilots, partnerships, or hiring.

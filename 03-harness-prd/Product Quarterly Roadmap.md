# RocketShip Roadmap — Q3 / Q4

Maintained by Product.

## Q3 — Committed

| Initiative | Pillar | Priority | Owner | Target | Notes |
|---|---|---|---|---|---|
| SAML/SSO for Okta | Enterprise-Readiness by Default | P0 | Security & Compliance | Oct 1 | Hard deadline, tied to Acme Corp. |
| Reporting export migration, phase 1 (async worker queue) | Trust at Scale | P0 | Platform & Infra | End of Q3 | First step toward fixing CSV export crashes. Does not unblock new AI load on the reporting table yet, that's Q4. |
| Q3 "AI story" prototype | Unmapped | Unscheduled | App & Frontend | Board meeting, end of Q3 | Gavin's ask, and now also apparently a line in a press interview he gave before this was scoped. Product found out about the press mention after the fact. |
| Dashboard visual refresh | Fast Time-to-Value | P3 | App & Frontend | Shipped early Q3 | Freed up App & Frontend capacity ahead of schedule. |

## Q3 — Not committed, but now something people expect anyway

| Initiative | Pillar | Priority | Owner | Notes |
|---|---|---|---|---|
| "Real-time Slack notifications" for pipeline failures | Unmapped | Unassigned | Unclear, possibly nobody | Surfaced by a sales rep on a call with Acme Corp, apparently as if it already exists. It does not. No engineering pod has scoped it or has capacity for it this quarter. Listed here so it's visible, not because it's planned. |

## Q4 — Planned, not yet committed

| Initiative | Pillar | Priority | Notes |
|---|---|---|---|
| Reporting table sharding (phase 2 of export migration) | Trust at Scale | P0 | Unblocks any AI feature that reads from or writes to the reporting database. |
| Admin panel permissions overhaul | Enterprise-Readiness by Default | P1 | Direct response to the Pearson Co "Error 403" incident. |
| Data lineage visualization | Trust at Scale | P2 | Slipped from Q3, Data Pipeline pod. |
| Webhook connector (customer-requested) | Fast Time-to-Value | P2 | Slipped from Q3, Data Pipeline pod. |
| Dark mode | Unmapped | P3 | Backlog. Repeatedly requested, never prioritized above P3. |
| Refresh onboarding email templates | Unmapped | P3 | Someone in Marketing asked for this in a hallway conversation. Not evaluated against anything above, just sitting on the list. |

# RocketShip Engineering Capacity Note — Q3

**From:** Priya Nair, VP Engineering
**To:** Product
**Re:** What we can actually take on this quarter

Product keeps asking what's "just a small AI feature." Here's where the four engineering pods actually stand right now, so we stop finding out about conflicts in sprint planning.

## Platform & Infra (6 engineers)

Almost entirely consumed by the legacy reporting API. Dave's team flagged it again this week: the CSV export service is throwing 500s on anything over 50MB, and every enterprise account's export volume is climbing. We are migrating export to an async worker queue this quarter, and the underlying reporting table needs to be sharded before it can safely take more load.

Until that sharding work ships, this pod cannot take on any feature that adds new read or write volume against the reporting database. That includes AI summarization, AI-generated reports, or anything else that queries reporting data on a schedule or in a loop.

## Security & Compliance (3 engineers)

Fully allocated to SAML/SSO for Okta. This is the Acme Corp blocker, and Compliance has told us it's non-negotiable P0 work. Nothing displaces it before it ships. Practical effect: this pod has no bandwidth this quarter to review new permission models or anything touching authentication, including whatever access an AI feature might need.

## Data Pipeline (4 engineers)

Roughly 30% slack capacity, mostly because two roadmap items slipped to Q4 already. One thing I only found out about yesterday, from a customer call I wasn't even supposed to be on: apparently a rep told Acme Corp that we have "real-time Slack notifications" for pipeline failures. We do not have this. Nobody on this team scoped it, nobody asked us, and I only know because I happened to be looped in on the call notes. If someone has committed to that in writing, we need to know now, not when it shows up as a signed contract line item in Q4.

Also, heads up that Marcus is out on parental leave through the end of the month. Anything routed through him on this pod will move slower than usual. Not related to the above, just don't be surprised.

## App & Frontend (5 engineers)

The pod with the most genuine slack, roughly 35%, after the dashboard visual refresh shipped early. This is where most "AI feature" prototypes actually get built, including whatever comes out of Gavin's "Magic Button" ask. Worth knowing: Gavin apparently mentioned an "AI-powered dashboard" in a press interview two weeks ago, before anyone here had scoped anything. We are now fielding questions from a reporter's follow-up email about a feature that doesn't exist yet. This pod would like it on the record that "make it pop" is not a spec.

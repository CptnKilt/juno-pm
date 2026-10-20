# Raw Signals

Five unrelated inputs that landed in the same week. Nobody has synthesized these yet.

## Artifact 1: User Interview Transcript

**Interviewer:** So, tell me about your workflow.

**User (Sarah, Data Analyst):** Honestly, it's been a week. My dog has been barking all morning, sorry if you hear him. Anyway, I log into RocketShip every Monday. The first thing I notice is that the new blue navigation bar is really bright, like hurts my eyes bright. Can we change that? But yeah, so I go to the "Quarterly Reports" tab. I select my date range, usually last 90 days, and hit "Generate PDF." That works fine. But then, and this is the part that makes me want to scream, I try to click "Export to CSV" because I need to pivot this in Excel. It spins for like 5 minutes and then just crashes. No error message. Just blank. I've lost hours because of this. I end up just taking screenshots of the table, which is stupid. Oh, and I'd love a dark mode.

## Artifact 2: Support Ticket

**Subject:** URGENT!!! SYSTEM IS BROKEN AGAIN
**From:** Mike Ross (Enterprise Account: Pearson Co)

Message: I AM SO SICK OF THIS. I have a board meeting in 20 minutes and I cannot access the user admin panel. Every time I try to add a new seat, it gives me "Error 403: Permissions Denied." I AM THE ADMIN. Why does your system think I don't have permissions?? We pay you guys $50k a year for this? Fix it NOW or I am calling my rep to cancel. Also, where is the invoice for last month? I can't find that either. UNACCEPTABLE.

## Artifact 3: Executive Email

**From:** Gavin Belson (CEO)
**To:** Product Team
**Subject:** AI Features

Team, I just saw what our competitor launched. They have a "Magic Button" that writes emails for users. We need to have an AI story for the Q3 release. I don't care exactly what it does, but it needs to feel magical. Maybe it summarizes the dashboard? Or predicts revenue? Let's get a prototype up by Friday. We need to show innovation. Make it pop.

Gavin

## Artifact 4: Sales Rep Call Notes (from CRM)

**Account:** Acme Corp (Prospect)
**Rep:** Jessica L.

Notes: Good call today. They really liked the dashboard visuals. The VP mentioned they are currently using Salesforce for this but want to switch to RocketShip for the speed. ONE MAJOR BLOCKER: They absolutely cannot sign unless we have SAML/SSO support for Okta. Their security compliance requires it. If we can't ship SSO by Oct 1st, the deal is dead. Also, they asked if we can integrate with TikTok? I told them maybe. Let's look into it.

## Artifact 5: Slack Thread

**User:** dev_dave
**Channel:** #backend-monitoring

Message: Heads up, the legacy reporting API is redlining again. If we push any more volume to the CSV export service without refactoring the queue, the whole thing is gonna tip over. I'm seeing 500 errors on requests larger than 50MB. We need to migrate to the async worker ASAP, or at least cap the export size. We definitely cannot add any new "AI summarization" features on top of this DB until we shard the table. It's too fragile.

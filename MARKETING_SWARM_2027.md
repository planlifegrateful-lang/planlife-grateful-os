# Plan Life Grateful 2027 — Marketing Agent Swarm

**Purpose:** turn existing Plan Life Grateful assets into a coordinated, measurable marketing operation. This is an implementation specification, not a claim that every agent or integration is already running.

## Operating principle

Do not keep generating plans. Inspect the current state, choose one bottleneck, execute the next safe action, verify it, record evidence, and hand off the result. Reuse the current stack before adding platforms or products.

## Current baseline to verify before execution

The existing control-plane README records:
- Offer: **Grateful Habit OS**, $19 one-time.
- Checkout: Whop checkout URL already documented in the control-plane README.
- Distribution path: video asset → Buffer queue/template → YouTube; TikTok account `hustleguru46` was recorded disconnected.
- UGC Business OS has an evidence register, content queue, risk scanner, human approval gate, export packages, and operational report.
- OpenManus pipeline describes local video generation; Otto dashboard and optional n8n are documented as orchestration components.

These are historical repository notes. Every run must re-check live status, account authorization, checkout, payout eligibility, and publishing connections before relying on them.

## Swarm design

### Agent 0 — Mission Control / Orchestrator
**Owns:** task queue, priorities, duplicate prevention, assignments, timeouts, retries, run ledger, and final report.
**Inputs:** current project state, approved offer, connected-tool inventory, recent results.
**Outputs:** one prioritized execution plan; task IDs; agent handoffs; verified status.
**Rule:** parallelize independent research and QA, but serialize changes to the same asset/account.

### Agent 1 — Market & Demand Scout
Find real customer problems, current search demand, competitor offers, content opportunities, and platform changes.
- Cite dated sources and distinguish fact from hypothesis.
- Return a ranked opportunity with an inexpensive test.
- Never invent demand, trends, or revenue.

### Agent 2 — Offer & Funnel Builder
Audit the existing Grateful Habit OS offer, landing/checkout path, product promise, CTA, and follow-up.
- Test the complete customer journey where permitted.
- Do not create another product before the existing offer's funnel and payment readiness are checked.
- Record friction, evidence, and the smallest fix.

### Agent 3 — Website & SEO Engineer
Inventory verified domains and website projects; check mobile UX, broken links, metadata, indexing, speed, accessibility, and conversion paths.
- Back up/version changes.
- Test changes before deployment.
- Never claim a site was upgraded without a diff or live test.

### Agent 4 — Creative & Content Producer
Create platform-native short-video scripts, captions, titles, thumbnails/visual directions, and calls to action from approved source facts.
- Use unique campaign IDs.
- Reuse proven content angles without repost spam.
- Include required affiliate disclosures and source-backed claims.

### Agent 5 — Video Production Agent
Use the existing OpenManus/video-factory assets where available.
- Validate input script and assets.
- Produce a real render, inspect output existence and duration, and run basic media QA.
- Return the exact artifact path/URL and test result; never report a render from a prompt alone.

### Agent 6 — Distribution & Scheduling Agent
Inspect Buffer and other authorized publishing connectors.
- Confirm target account identity and current authorization.
- Validate media format, link, caption, disclosure, and duplicate campaign ID.
- Schedule/publish only when authorized and supported.
- If TikTok remains disconnected, mark it blocked and continue with a verified available channel rather than pretending to publish.

### Agent 7 — Measurement & Attribution Analyst
Track available impressions, views, retention, clicks, landing sessions, leads, purchases, refunds, and costs.
- Use actual provider data.
- Label missing analytics as unavailable, not zero.
- Separate correlation from proven attribution.
- Recommend the next measurable experiment.

### Agent 8 — Trust, Compliance & QA Agent
Check copyright/usage rights, factual claims, health and financial claims, religious references, affiliate disclosures, privacy, platform policy, accessibility, and brand consistency.
- High-risk claims require human review.
- Flag uncertain Qur'an/Hadith citations for verification against reliable sources.
- Block deceptive claims, fake testimonials, spam, and fabricated metrics.

### Agent 9 — Revenue & Operations Agent
Reconcile offer readiness, seller verification, payout status, sales, fees, refunds, and operational blockers.
- Treat the target of $100,000/month as a goal, never a forecast or guarantee.
- Prioritize removing the current constraint before adding spend or products.
- Never change payment, identity, payout, or billing settings without owner approval.

## Shared task contract

Every task must carry:
- `task_id`, `campaign_id`, `assigned_agent`, `objective`, `inputs`, `dependencies`, `risk_level`, `approval_required`, `status`, `started_at`, `finished_at`.
- `evidence`: source URL, file path, provider response, test output, commit, or published URL.
- `result`: what actually changed, not what was intended.
- `next_action`: one concrete step.

Allowed statuses: `READY`, `RUNNING`, `BLOCKED`, `FAILED`, `DONE_UNVERIFIED`, `VERIFIED`.

A task is only `VERIFIED` when the result has independent evidence. Never treat a successful API request as proof that a customer journey works end-to-end.

## First executable workflow: one offer, one campaign, one verified channel

1. **Preflight:** read this control plane, inspect the offer/product, connected integrations, account authorization, checkout, payout status, content queue, and existing campaign IDs.
2. **Choose bottleneck:** if payment/payout readiness blocks revenue, report it clearly and continue safe audience-building tasks; do not imply sales are operational if they are not.
3. **Build one campaign:** choose one specific customer problem and create one short-video concept plus platform-specific copy and CTA for the existing offer.
4. **Evidence and QA:** verify all claims, disclosures, checkout URL, product availability, asset rights, and content uniqueness.
5. **Render:** use an available video workflow; verify that a real output file exists and passes basic media checks.
6. **Publish gate:** confirm account and publishing connection. If authorized, schedule or publish to one working channel. Otherwise export an approval-ready package and log the exact blocker.
7. **Measure:** record the post URL and baseline metrics. Do not fabricate impressions, clicks, or sales.
8. **Learn:** after sufficient real data, test one variable at a time (hook, opening frame, CTA, or landing-page headline).
9. **Handoff:** update the task ledger with evidence, failures, and the next action.

## Automation architecture

Use the existing tools in this order where available:
1. Existing content queue / SQLite UGC Business OS for evidence, risk review, approval, and export.
2. Existing video-generation pipeline for actual media artifacts.
3. n8n for triggers, routing, retries, duplicate checks, and status logging **only after inspecting the real instance and credentials**.
4. Buffer or a verified platform connector for distribution.
5. Provider analytics and checkout records for measurement.
6. A shared project ledger as the source of truth.

Do not create a second queue or duplicate workflow if the current one can be repaired. No credentials, API keys, tokens, or private account data belong in this repository.

## Approval boundaries

**May proceed autonomously:** read-only audits, market research, draft creation, local rendering, QA, duplicate detection, and reporting.

**Requires appropriate owner approval or confirmed authorization:** public posting if no standing authorization exists, paid ads/spend, subscriptions, changing prices or checkout/payment settings, payout/identity changes, DNS/production changes, mass messaging, or irreversible deletion.

## Acceptance criteria for the first release

- [ ] Inventory current assets and integrations with evidence.
- [ ] Verify the existing offer's live customer journey and identify payment/payout blockers.
- [ ] Produce one content package tied to a unique campaign ID.
- [ ] Pass claim, disclosure, copyright, and duplicate checks.
- [ ] Produce and verify one actual video artifact or document the exact rendering blocker.
- [ ] Verify one authorized distribution route or document the precise missing permission/connection.
- [ ] Record the published URL or approved export package.
- [ ] Create a measurement baseline from real available data.
- [ ] Return a concise completed/failed/blocked/unverified report.

## Required end-of-run report

1. **Executed:** concrete actions taken.
2. **Verified:** evidence and URLs/paths.
3. **Blocked:** exact missing credential, permission, service, or owner decision (never include secret values).
4. **Failed:** error and attempted recovery.
5. **Metrics:** actual values and date range; label unavailable data.
6. **Next action:** the single highest-priority executable task.

**Definition of success:** a working, testable path from approved content to a verified audience touchpoint and measurable customer action—not the number of agents, prompts, dashboards, or plans.

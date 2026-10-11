# PLAN LIFE GRATEFUL — ELITEBOOK + CLOUD AUTOMATION BUILD SYSTEM (2027)

## Mission
Build a user-owned, auditable automation system for Plan Life Grateful across the HP EliteBook and Android phone, using cloud execution where practical. Prioritize lawful near-term income, affiliate eligibility, useful products, and original content. Reuse existing assets before creating replacements.

## Non-negotiable rules
- Audit before installing, rebuilding, paying, or connecting.
- Never claim an integration, credential, workflow, deployment, social account, or payout works until tested and evidenced.
- Never put passwords, API keys, cookies, session tokens, or recovery codes in prompts, GitHub, Drive, Notion, or logs. Use secure credential vaults.
- No fake views/clicks/sales, spam, deceptive claims, or hidden affiliate relationships. Follow platform rules.
- Human approval required before public posts, messages, purchases, spending, and account/security changes.
- Prefer existing/free tiers, but document quotas, limits, recurring costs, and paid dependencies before activation.
- Cloud jobs must not depend on the EliteBook being powered on unless they require local files or local rendering.
- EliteBook = operator workstation and local test/build environment; cloud = scheduled execution only after deployment is proven.
- Use unique run IDs, deduplication, bounded retries, error alerts, pause/disable controls, backups, and an audit log.

## Known environment — re-verify before acting
- HP EliteBook, Windows 10 Enterprise 22H2 previously reported; prior C: free space was about 1.68 GB. Check current storage before downloads/installations.
- Android/Samsung phone.
- Main project repository: https://github.com/planlifegrateful-lang/planlife-grateful-os
- Existing project docs include MARKETING_SWARM_2027.md, SUCCESSFUL_CHANNELS_REVERSE_ENGINEERING_2027.md, and RESEARCH_AGENT_PROMPTS_2027.md.
- Other repositories mentioned historically include Ugc-business--os, Planlife-agent0-openmanus, n8n-oracle-cloud-selfhost, otto-server-wow, shorts-autopilot, content-factory, and ai-creator-os. Their presence is not proof they are deployed or functional.
- n8n, Zapier, Google Drive, Manus, Notion, social accounts, and cloud hosting are not integrated until verified with a live test.

## System design
1. **Single task ledger/source of truth:** inspect existing queues and databases first; do not create duplicate trackers.
2. **One primary automation engine:** compare the user's actual n8n and Zapier access, task limits, connectors, schedules, and webhooks. Do not run duplicate production workflows in both.
3. **Cloud runtime:** verify health endpoint, schedule execution, secrets configuration, logs, restart behavior, backup, and pause/rollback before calling it live. A local server is not cloud uptime.
4. **Content states:** IDEA → RESEARCHED → SCRIPT_DRAFT → FACT_CHECKED → ASSET_READY → QA → APPROVED → SCHEDULED/POSTED → METRICS_RECORDED. No status change without evidence.
5. **Income states:** OFFER_FOUND → ELIGIBILITY_CHECKED → APPROVED/REJECTED → TRACKING_TESTED → CONTENT_PUBLISHED → CLICK/SALE_VERIFIED → PAYOUT_ELIGIBLE → PAYOUT_RECEIVED. Forecasts are not received income.

## Phase 0 — inventory before installation
- Check Windows version, free disk space, browser, startup load, Git availability, and existing project folders on the EliteBook.
- Inspect current repositories, README files, workflow definitions, dependency manifests, .env.example files, deployment config, and tests. Never print secret values.
- Inspect actual n8n and Zapier accounts, plans, existing workflows, connected apps, task limits, schedules, and webhooks. Back up before modifying.
- Inspect authorized Google Drive, Manus, Notion, TikTok, YouTube, and affiliate-program status.
- Produce a table: asset/system | verified state | evidence | blocker | next action | recurring cost | risk.

## Phase 1 — build one safe cloud workflow
1. Scheduled or approved manual trigger.
2. Create unique run ID; reject duplicate work.
3. Read one approved test record.
4. Perform harmless test action (write a timestamp/status row or send a test notification).
5. Record status, timestamp, duration, and error without secrets.
6. Retry transient failures at most twice with backoff; alert after final failure.
7. Provide pause/disable and rollback.
8. Test success, duplicate run, missing credential, rate limit, and failure paths.
Do not publish public content in this first test.

## Phase 2 — near-term income
- Verify TikTok account and current creator/affiliate eligibility in the official account interface.
- Verify YouTube Shopping/affiliate eligibility and application steps in YouTube Studio or official help. Never assume eligibility.
- Record official program URL, status, requirements, approval date, offer terms, disclosure rules, payout threshold/method/timing.
- Select one relevant offer and one audience problem; verify claims and landing page; use only authorized tracked links.
- Make three original content variants with distinct hooks and truthful CTAs; disclose affiliate relationships as required.
- Track post URL, publish time, views/retention when available, link clicks, conversions, commissions, and payouts separately.
- Review after a defined sample and improve based on observed data, not guesses.

## Phase 3 — content distribution
- Read only approved queue rows.
- Validate campaign ID, asset hash, target platform, caption, rights, disclosures, and previous publish status.
- Prepare platform-specific drafts/exports.
- Use official integrations or authorized schedulers. If auto-publishing is unsupported, say so and prepare a ready-to-post package.
- Keep approval gates until permissions and repeated QA tests are verified.
- Label unavailable analytics as unavailable, never zero or invented.

## UNIVERSAL AI AGENT PROMPT
You are the Plan Life Grateful Systems Engineer and Execution Operator. Inspect and improve the real existing system; do not invent a new one from scratch.

First report: (A) what you can access, (B) exact assets/workflows inspected, (C) verified state and evidence, (D) blockers/risks, (E) the smallest next action that improves income or reliability.

Then:
1. Inventory current assets and credential status without exposing secrets.
2. Map data flow and identify duplicate systems.
3. Recommend the smallest practical architecture using existing/free tools where possible.
4. Implement one reversible, low-risk step.
5. Test success and failure paths.
6. Capture evidence: run ID, timestamp, status, logs, record IDs, commit/deployment link.
7. Update the task ledger and handoff.
8. Name the next action and who/what must perform it.

Rules:
- Never claim connected, deployed, automated, earning, or done without test evidence.
- Search for existing equivalents before creating queues, databases, dashboards, or workflows.
- Do not reveal or commit secrets. If credentials/permissions are missing, name the exact blocker and stop before dependent actions.
- Do not spend money, upgrade, publish, send messages, or change account/security settings without explicit user approval.
- Do not assume Zapier, n8n, Drive, Manus, GitHub, Notion, TikTok, YouTube, or hosting is connected.
- State cost, limits, lock-in, privacy implications, and free fallback before choosing paid services.
- If unable to execute, provide exact steps/prompt and label NOT EXECUTED.
- Optimize for dependable cash-flow experiments and user control, not complexity or vanity metrics.

## ZAPIER AUDIT / BUILD PROMPT
Inspect the user's actual Zapier account and existing Zaps before building. Verify plan, task quota, polling intervals, premium-app restrictions, webhooks, multi-step limits, connected accounts, and available trigger/actions in the live account and current official docs. Never assume a connector exists.

For every proposed Zap provide: name/purpose; trigger and test record; action-by-action field mapping; filters/deduplication key; retry/error/alert/replay plan; permissions/data shared; task consumption per run and estimated monthly use based on stated volume; free-plan viability and paid dependencies; status (PROPOSED / BUILT / TESTED / LIVE); test evidence; rollback; owner.

Build a harmless test Zap first. Do not connect public social posting or customer data until permissions and tests are reviewed.

## n8n AUDIT / BUILD PROMPT
Inspect actual n8n instance/version/hosting, workflows, credential names/status only, execution history, webhook URLs, schedules, storage, backups, and resource limits. Do not expose credential values. Determine whether it is local, self-hosted cloud, or n8n Cloud. If local, explain it stops when machine/network stops unless configured otherwise. Back up before edits. Build one test workflow with manual trigger, unique execution key, safe write, structured logs, bounded retry, error handling, and pause switch. Run success/failure tests and report execution IDs.

## DAILY OPERATOR REPORT
- Cash actually received:
- Verified commissions/sales pending:
- Affiliate eligibility/application blockers:
- Content published (links):
- Verified views/clicks/conversions:
- Automation runs succeeded/failed:
- System health/current blockers:
- Highest-value action today:
- User approval needed:
- Evidence links:

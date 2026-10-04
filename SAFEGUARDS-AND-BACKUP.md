# PHASE 5: SAFEGUARDS AND BACKUP

**Last updated:** 2026-10-04

## 1. 2FA Status (you complete the codes)

| Account | 2FA Enabled | Notes |
|---------|-------------|-------|
| GitHub (planlifegrateful-lang) | [ ] | |
| Whop (Limitless UGC) | [ ] | |
| Buffer | [ ] | |
| Google / Drive | [ ] | |
| Outlook | [ ] | |
| Make.com (if used) | [ ] | |
| Notion | [ ] | |

Enable 2FA on every account today. Codes stay with you.

## 2. Kill Switch — Pause Everything in Under 60 Seconds

### Automations (Grok)
1. Call automation_list (or open the Automations UI).
2. For every active task: set is_enabled = false on the schedule_id (or pause the whole task_id).
3. Priority order: MONEY MOVE 1 → Daily Command → MONEY MOVE 2 → Systems Upgrade → Outlook → Webhook.

Exact taskIds for instant reference:
- MONEY MOVE 1: 02355977-29e9-443d-9746-2ecf29e27242
- Daily Command: 43b6b866-11ce-4cfd-9d2c-a7a3c27d8e24
- MONEY MOVE 2: 2916b1ad-1178-4a42-bf70-db5388f4d743
- Systems Upgrade: b5826650-1c6f-44ef-8ccb-29474e907493

### Buffer
- Open Buffer → Queue → Unschedule All / Clear scheduled posts.

### Content Draft Scenarios (Make.com / Claude)
- Leave OFF by default. Turn on only after manual review of the three assets.

### Result
All scheduled content, daily briefs, and event triggers stop within one minute.

## 3. Weekly Export Procedure

Every Sunday or Monday:
1. Export full automation_list JSON (or screenshot + list).
2. Export Vault / Master Index sheet (or this repo’s MASTER-INDEX.md).
3. Save both to Google Drive folder: `PlanLifeGrateful / Weekly-Backups / YYYY-MM-DD`.
4. Optional: git tag the control plane repo `backup-YYYY-MM-DD`.

## 4. Activity Log Template

Add a new row every significant action:

| Date | Platform | Action | Result | Operator |
|------|----------|--------|--------|----------|
| 2026-10-04 | Automations | Refreshed MONEY MOVE 1 + Daily Command + Systems Upgrade schedules | nextRun moved to current day/week | Master Operator |
| 2026-10-04 | GitHub | Locked planlife-grateful-os + grateful-life-plan READMEs to $19 checkout | Source of truth fixed | Master Operator |
| | | | | |

Copy this table into Notion, Google Sheet, or keep appending in ACTIVITY-LOG.md.

## 5. Vault Sheet Structure (create once)

Google Sheet or Notion database named **Vault**:

Columns:
- Date
- Platform (YouTube / Facebook / TikTok / Buffer / Whop)
- Asset Type (Short script / Caption / Link-hub / Pin)
- Title / Hook
- Status (Draft / Private / Published / Archived)
- Checkout URL used
- Notes / Compliance check
- Link to file or video

Every Claude / Make.com draft logs one row here before any upload.

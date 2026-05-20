# Application tracker template

## Single source of truth

Maintain ONE tracker — a Google Sheet or markdown table — as the source of truth. Update it every time something changes.

## Sheet structure

### Tab 1: Active Hit List

| Tier | Status | Company | Role | Path | Location | Comp Est All-In | Warm Contact (Tier) | Hiring Manager | Apply URL | Next Action | Date Added | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

**Tier values:**
- 1 - ACTIVE (applied or outreach in flight)
- 2 - APPLY THIS WEEK
- 3 - WARM-LED WATCH (no current open role, ping warm contact for intel)
- 4 - CONDITIONAL (need to verify something before applying)
- RULED OUT (with reason in Notes)

**Status values:**
- Applied [date]
- Outreach in flight
- Identified
- Conditional
- Watch + intel ping
- Killed

**Path values:**
- A (aspirational / Path A)
- B (safety / Path B)

### Tab 2: Outreach Loops

| Action | Owner | Recipient | Sent Date | Awaiting | Next Step Date | Notes |
|---|---|---|---|---|---|---|

Track every outreach that's "in flight" — LinkedIn DMs, emails, recruiter follow-ups. Set a Next Step Date for when to nudge if no reply.

### Tab 3: Open Questions Blocking Action

| Question | Why It Matters | Owner |
|---|---|---|

E.g., "Confirm Squarespace remote policy — gates whether to apply"

### Tab 4: Ruled Out (with reasons)

Preserve history. Don't re-evaluate the same role next month.

| Date Ruled Out | Company | Role | Reason |
|---|---|---|---|

## Update cadence

- **Daily during active search:** mark applications, log responses, update next steps
- **Weekly:** add new finds from aggregator sweep, prune stale leads
- **Per conversation:** capture what was learned, update tier

## Naming convention

If creating multiple versions (which Google Drive MCP requires since there's no edit-in-place):
- `Master Hit List v1` → deprecated as v2 lands
- `Master Hit List v2` (current)

Always rev the version when the structure changes. Keep old versions in the folder for audit history.

## Sample row (illustrative — fill in your own data)

```
2 - APPLY THIS WEEK | Identified | [Company] | [Role Title] | B | [Location] |
[$XXX-YYY all-in] | [Contact Name] ([their title], [year connected]) - [tier: High/Med/Low/cold] |
TBD - need 2nd-degree research | [Apply URL] |
Cold app this week + scope 2nd-degree path | [Date Added] |
[Brief notes on why this role fits + any risks]
```

# Resume tailoring framework

## Principles

1. **Surgical edits, not rewrites.** 4–6 find/replace blocks per role. Not a new resume.
2. **Match the JD's exact keywords.** ATS keyword-scans first. If the JD says "AI go-to-market strategy," the user's resume should say "AI go-to-market strategy" — not "GenAI positioning."
3. **Keep formatting intact.** Don't disrupt the user's chosen layout. Give them text edits to paste.
4. **Don't over-stuff.** Resume readability matters. If a JD has 30 keywords, surface the top 5–7.
5. **Redact confidential current-employer details when applying to competitors.** Especially in-beta products, internal initiatives, monetization mechanics, etc.

## Process per role

### Step 1: Audit the JD

Extract:
- Required experience years
- Top 5–7 keywords/phrases
- Function name (Brand Marketing vs Creative Ops vs PMM etc.)
- Reporting structure
- Team scope (managing # people, ICs vs managers)
- Compensation if shown

### Step 2: Audit the user's resume against the JD

For each JD keyword, find where it lives (or doesn't) in the user's resume.

| JD keyword | Where it could land |
|---|---|
| AI go-to-market strategy | Adobe bullet about GenAI feature tiers |
| Multi-brand portfolio | Adobe bullet about Express + Firefly portfolio |
| 15+ years | Summary line |
| Scaled team management | Booksy 15-person org / Adobe 6-person team |

### Step 3: Identify the gaps

Common gaps:
- **JD keyword present in user's experience but missing from resume language** → easy edit
- **JD keyword present in user's experience using a different phrase** → reframe edit
- **JD keyword genuinely missing from user's background** → don't fabricate. Flag as a stretch in the interview prep instead.

### Step 4: Write the surgical edits

Format every edit as a find/replace block the user can apply in 30 seconds:

```
EDIT N: [section name]

FIND: [exact text from current resume]

REPLACE WITH: [new text that surfaces JD keywords]

WHY: [one sentence on what this accomplishes]
```

### Step 5: Limit to 4–6 edits

Pick the highest-impact 4–6. Don't surface 12 edits.

## Edit types ranked by impact

1. **Headline** (under name) — first thing read; high impact for ATS keyword match
2. **Summary paragraph** — second thing read; surfaces narrative arc
3. **Skills section line additions** — keyword matching
4. **Current role bullets** — most-recent experience carries the most weight
5. **Bullet reorder within a section** — putting strongest metric first
6. **Old role context line** — for older roles, the context line matters more than bullets

## Anti-patterns

❌ **Don't write entirely new bullets.** Edit existing language.
❌ **Don't add metrics the user didn't actually achieve.** Resume integrity matters.
❌ **Don't strip personality.** If the user's voice comes through in current bullets, keep it.
❌ **Don't surface confidential current-employer details to competitors.** If the user is at Co A and applying to Co B which is a competitor, redact any in-beta product details, internal monetization mechanics, etc.
❌ **Don't over-edit.** If the resume already maps to 80% of the JD, do 2 small edits — not 6.

## Per-role tailoring vs Master resume

Pattern: keep a master resume (the user's "longest, most-truthful version"). For each role, derive a tailored version via 4–6 edits.

Recommend the user save tailored versions as separate docs:
- `Resume_Master_v3.md` (master)
- `Resume_Master_v3_Norton.md` (Gen Norton-tailored)
- `Resume_Master_v3_Calendly.md` (Calendly-tailored)
- etc.

## Self-audit after edits

After delivering the edits, audit your own work:
- Does the resume now actually map to the JD? Or did you just keyword-stuff?
- Did you redact confidential details if applying to a competitor?
- Are the edits surgical (≤ 6) or did you over-deliver?
- Is the user's voice intact?

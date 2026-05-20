# Job aggregator rotation

LinkedIn-only is a coverage gap. Run this full rotation each sweep.

## Works via WebFetch (Claude can drive)

| Aggregator | URL pattern | Notes |
|---|---|---|
| **LinkedIn Jobs aggregator** | `linkedin.com/jobs/search/?keywords=...&location=...&f_TPR=...` | Use `f_TPR=r604800` for past week, `r2592000` for past month. Best fresh-listings source. |
| **Built In SF / NY / LA / National** | `builtin.com/jobs/...?sort=recent` | Server-rendered, accessible. SF tech-focused. |
| **Indeed** | `indeed.com/jobs?q=...&l=...&fromage=7` | Works but noisy. |
| **HackerNews "Who's Hiring"** | `news.ycombinator.com/...` | Monthly thread, first of the month. Sometimes rate-limited (429). |

## Blocked to Claude — user needs to relay

| Aggregator | Why blocked | Workaround |
|---|---|---|
| **Welcome to the Jungle** (welcometothejungle.com) | Auth wall to WebFetch | User logs in via browser. Either uses side-panel Claude on the search page, OR copies listings as text back to Claude. |
| **Lenny's Newsletter Job Board** (jobs.lennysnewsletter.com) | Redirects to pallet.xyz which is blocked | User skims manually. Curated for PMM/Product/Growth — high signal. |
| **Wellfound (ex-AngelList Talent)** | JS-rendered, blocked | User uses browser. |
| **YC Work at a Startup** (workatastartup.com) | Chrome MCP allowlist blocks | User opens tabs + uses side-panel Claude to extract listings. |
| **VC portfolio job boards** (a16z, Sequoia, Greylock, Index, Kleiner, Bessemer, Accel) | All JS-rendered + Chrome MCP allowlist blocks | User skims via browser + relays. Curated for portfolio cos. |
| **ExecThread** | Paid/auth-walled | User subscribes if relevant. |

## Search engines (Google, Bing, DuckDuckGo)

**All bot-block Claude's WebFetch.** Don't rely on web search for role discovery. If the user finds a role via Google search themselves, paste the URL to Claude for JD analysis.

## How to use the rotation

1. **Run the "works via WebFetch" set in parallel** at the start of each sweep
2. **Filter results** through the user's hard exclusions before showing them
3. **Ask the user to relay** the auth-walled aggregators each week — give them specific prompts to use with their browser's Claude side-panel
4. **For VC portfolio boards specifically:** the user opens 4–6 tabs (a16z, Sequoia, Greylock, YC) and uses side-panel Claude on each to list "every Director+ marketing/growth/relevant-function role visible — company, title, location, URL." Paste the lists back. Claude filters.

## Frequency

- **Daily during active search:** LinkedIn (week filter), Built In (recent sort)
- **Weekly:** Indeed, HackerNews Who's Hiring (if it's the right time of month), Welcome to the Jungle (via user), Lenny's (via user)
- **Bi-weekly:** VC portfolio boards (via user)

## What good looks like

A well-run sweep surfaces ~5–10 fresh roles per week that survive the user's filter. If you're regularly surfacing 20+ "fits," the filter is too loose. If you're regularly surfacing 0–1, the filter is too tight or the search is too narrow.

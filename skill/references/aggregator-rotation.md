# Job aggregator rotation

**Don't waste time on individual company careers pages** — they're slow, JS-rendered, often blocked. Use aggregators. Pick the right ones for the user's specific function.

## Function-specific aggregator map

### Marketing senior leadership (PMM, Brand, Growth, Lifecycle, Creative Ops)

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | `linkedin.com/jobs/search/?keywords=X&location=Y&f_TPR=r604800` | Best fresh-listings source. Week filter = `r604800`, month = `r2592000` |
| **Lenny's Newsletter Job Board** | `jobs.lennysnewsletter.com` (redirects to pallet.xyz/list/lennys-jobs) | Curated, senior PMM/Growth-heavy, high signal. Redirect → pallet.xyz which can be blocked to AI. User may need to skim manually. |
| **Built In** | `builtin.com/jobs/sf/marketing` (or `/ny`, `/la`) | Server-rendered, accessible. Tech-heavy. |
| **Welcome to the Jungle** | `welcometothejungle.com` | Auth wall to AI. User logs in via browser, pastes listings back. |
| **Wellfound** (formerly AngelList Talent) | `wellfound.com/jobs` | Auth wall. Startup-heavy. |

### Product Management

| Aggregator | URL | Notes |
|---|---|---|
| **Lenny's Newsletter Job Board** | `jobs.lennysnewsletter.com` | Lenny is a PM by background — highest signal for senior PM roles |
| **Mind the Product Job Board** | `mindtheproduct.com/jobs` | PM-specific community |
| **LinkedIn Jobs** | (as above) | |
| **Y Combinator Work at a Startup** | `workatastartup.com` | Auth wall + JS-rendered. User must skim manually. |
| **Built In** | (as above) | |

### Engineering (IC + Management)

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **Hacker News "Who's Hiring"** | `news.ycombinator.com` (monthly thread, first of month) | Best startup engineering source. Sometimes rate-limited. |
| **YC Work at a Startup** | `workatastartup.com` | Auth wall but high signal |
| **Wellfound** | `wellfound.com/jobs` | Auth wall |
| **Levels.fyi** | `levels.fyi` | NOT a job board — comp benchmarking critical for offer negotiation |

### Design (Product / UX / Visual / Brand Design)

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **Dribbble Jobs** | `dribbble.com/jobs` | Design-specific, high signal |
| **Working Not Working** | `workingnotworking.com` | Senior design + creative community |
| **Coroflot** | `coroflot.com/jobs` | Industrial + product design |
| **AIGA Design Jobs** | `designjobs.aiga.org` | |
| **Built In** | (Creative section) | |

### Brand / Creative Operations / Creative Director / Production

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **Built In** | (Creative section) | |
| **Welcome to the Jungle** | (as above) | |
| **Working Not Working** | `workingnotworking.com` | |
| **IfYouCouldJobs** | `ifyoucouldjobs.com` | UK-heavy but some US |

### Sales / Customer Success / Revenue

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **RepVue** | `repvue.com/jobs` | Sales-specific + employer ratings |
| **Bravado** | `bravado.co` | Sales community + jobs |
| **Built In** | (as above) | |

### Program Management / TPM / Operations / Chief of Staff

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **Wellfound** | (as above) | |
| **Built In** | (as above) | |
| **Welcome to the Jungle** | (as above) | |
| **Pallet (Chief of Staff curated)** | `pallet.xyz` (search for CoS lists) | Several CoS-specific lists curated on Pallet |

### Data / ML / AI Research

| Aggregator | URL | Notes |
|---|---|---|
| **LinkedIn Jobs** | (as above) | |
| **Hacker News "Who's Hiring"** | (as above) | |
| **YC Work at a Startup** | (as above) | AI-heavy of late |
| **Wellfound** | (as above) | |
| **Kaggle Job Board** | `kaggle.com/jobs` | Data science specific |

## Browser access guidance

### Works via WebFetch / standard AI tool access:

- LinkedIn Jobs aggregator (search URLs work)
- Built In (all locations)
- Indeed (`indeed.com/jobs?q=X&l=Y&fromage=7`)
- Hacker News (occasional 429 rate limit)
- Lenny's Newsletter (the email — Pallet redirect blocked)

### Auth-walled — user needs to relay

For each of these, the user logs in via their browser and either:
- (a) Pastes listings as text back to Claude, OR
- (b) Uses Claude in Chrome browser extension's side-panel feature

**Auth-walled boards:**
- Welcome to the Jungle
- Wellfound
- YC Work at a Startup
- VC portfolio boards (a16z, Sequoia, Greylock, Index, Kleiner) — also JS-rendered
- ExecThread (paid)

### Universally blocked to AI

- Google / Bing / DuckDuckGo search (bot-blocked)
- Most company careers pages (JS-rendered, slow, individually targeted)

**Don't waste time** on Google search — it doesn't work. Tell the user to either:
- Search Google themselves and paste interesting listings back
- Use the aggregator rotation above instead

## Browser extension recommendations for users

### Claude in Chrome (browser extension)

For users running Claude.ai or Claude Code, the **Claude in Chrome** extension adds a side-panel that can read whatever tab they have open. This is useful for:
- Auth-walled aggregators (user logs in, side-panel can read)
- VC portfolio job boards (side-panel can extract listings)
- Specific JDs that are blocked to WebFetch

Install: `claude.ai/download` → Chrome extension

### LinkedIn data exporter (no extension needed)

LinkedIn's native data export (Settings → Data Privacy → Get a copy of your data → Connections) gives the user a CSV of all their connections. Free, no extension. 10–30 min lag via email.

## How to use this rotation

1. **Identify the user's function** in Phase 1 of onboarding
2. **Pick the 3–5 most relevant aggregators** from the table above
3. **Run sweeps in parallel** using WebFetch or other tool access
4. **Auth-walled aggregators:** ask the user to relay
5. **Filter every result** against the user's hard exclusions before showing it to them
6. **Read JDs** for any role surfaced before adding to the hit list

## Frequency

- **Daily during active search:** LinkedIn (week filter), function-specific board with highest signal
- **Weekly:** Built In, Indeed, function-specific secondary boards
- **Bi-weekly:** Auth-walled aggregators (via user relay), VC portfolio boards (via user relay)
- **Monthly:** HN "Who's Hiring" thread (first of every month)

## What good looks like

A well-run sweep surfaces 5–10 fresh roles per week that survive the user's filter. If you're regularly surfacing 20+ "fits," the filter is too loose. If 0–1, too tight or too narrow.

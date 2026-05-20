# Career Search Coach — a Claude skill for serious job searches

A free, open-source job search coach built as a Claude skill. Designed for senior professionals running a strategic search — especially those who've been laid off, are facing a downlevel, or want to make a deliberate next move.

Works across functions: **Product Marketing, Product Management, Engineering, Design, Program Management, Operations, Brand & Creative, Sales, Customer Success** — anywhere title and function shape matter and where the job market is structurally noisy.

## What it does

Given your resume, your LinkedIn connections export, and a 15-minute strategic conversation, it gives you:

1. **A personalized hit list** of 10–15 verified-shape opportunities filtered against your actual function, level, comp floor, and lifestyle constraints
2. **Warm contacts surfaced** from your LinkedIn network at each target company, with explicit tier rankings (Tier 1 HM, Tier 2 peer, etc.)
3. **Surgical resume edits** per top role — find/replace blocks tailored to specific JDs, not generic advice
4. **Outreach drafts in your voice** — calibrated to how you actually write, not corporate-formal templates
5. **A tracker** as your single source of truth — applications, outreach in flight, ruled out (with reasons), open questions

## What makes it different

- **Honest filtering, not list-padding.** It will tell you when a role doesn't fit instead of inflating the list.
- **Function-shape matching, not keyword matching.** It distinguishes Product Management from Product Marketing, Engineering Manager from Staff Engineer, Brand Marketing from Creative Operations, Technical Program Manager from Product Manager. They're partner functions, not synonyms.
- **Verifies relationship tier.** A LinkedIn connection is not a warm contact. The skill explicitly asks you to confirm before treating someone as an intro path.
- **Knows when to push back.** If you're chasing a stretch role, asking a junior contact for an inappropriate senior referral, or about to send a "tone-wrong" outreach note, it'll flag it.

## How to use it

### Option A: Claude Code (install as a skill)

If you use Claude Code:

1. Clone or download this repo
2. Copy the `skill/` folder to `~/.claude/skills/career-coach/`
3. In Claude Code, type `/career-coach` to invoke

```bash
# From the repo root
mkdir -p ~/.claude/skills/career-coach
cp -r skill/* ~/.claude/skills/career-coach/
```

### Option B: Claude.ai or Claude desktop app (no install)

If you use Claude.ai in the browser or the Claude desktop app:

1. Open the file [`STANDALONE_PROMPT.md`](STANDALONE_PROMPT.md)
2. Copy the entire contents
3. Paste it as your first message in a new Claude conversation
4. Then say: *"Let's start. I'm searching for [briefly describe your situation]."*

The standalone version condenses the skill into a single-file prompt that works in any Claude conversation.

### Option C: Any AI assistant (ChatGPT, Gemini, etc.)

The framework and reference docs are model-agnostic. You can paste `STANDALONE_PROMPT.md` into any modern LLM and walk through the same process. Claude tends to follow the function-shape matching and voice rules more closely; mileage may vary on others.

## What you'll need

- Your resume (PDF, DOCX, or markdown)
- Your LinkedIn connections export ([instructions in skill/references/linkedin-export-howto.md](skill/references/linkedin-export-howto.md)) — takes 10 minutes
- 30–60 minutes for the first onboarding conversation
- A Google Drive / Sheets account if you want the auto-generated tracker

## Who this is for

This skill is most useful for:

- **Senior individual contributors** (Staff/Principal Engineer, Sr/Principal PM, Sr/Principal Designer, Sr PMM) navigating a competitive senior market
- **Managers and Directors** (EM, Design Manager, Director Product, Director Marketing, etc.) where title and scope matter and where promotion/lateral decisions affect long-term trajectory
- **VPs and Heads of function** running a strategic search where comp, brand, and proximity-to-power tradeoffs are real
- **People recently laid off** who need to act quickly without sacrificing fit
- **Anyone exploring a career pivot** between adjacent functions (e.g., PM ↔ PMM, EM ↔ Staff Engineer, Program Manager ↔ Chief of Staff) where understanding function boundaries determines what's a real option

Less useful for entry-level searches (the warm-contact and function-shape rigor matters less when you're optimizing for any-foot-in-the-door).

## Privacy

Everything runs locally with your own LLM account. The skill reads your resume and LinkedIn CSV inside your Claude conversation — nothing is sent to a third-party service. The author of this repo doesn't see your data.

## Contributing

Feedback welcome. If you run this skill and find a gap, an outdated reference, or a place where the function-shape matching is wrong, open an issue or PR.

## License

MIT — use it, fork it, improve it.

# Publishing Instructions

You have three publishing paths. Pick one based on your audience and how technical you want it to feel.

---

## Path A: GitHub (recommended — looks legit + works as a real skill)

**Audience:** Mix of technical + non-technical. Polished, professional, evergreen.

**Steps:**

1. **Create a free GitHub account** if you don't have one: [github.com/signup](https://github.com/signup)

2. **Create a new public repo:**
   - Click "+" → New repository
   - Name: `career-search-coach` (or `claude-career-coach`)
   - Description: "A strategic job search coach built as a Claude skill"
   - Public
   - Add a README ✓
   - License: MIT
   - Click "Create repository"

3. **Upload the files** (from this folder — `/Users/julianakatz/career-coach-skill/`):
   - Click "Add file" → "Upload files"
   - Drag the entire contents (README.md, STANDALONE_PROMPT.md, skill/ folder)
   - Commit message: "Initial release"
   - Commit

4. **Your link will be:** `https://github.com/YOUR-USERNAME/career-search-coach`

5. **Paste this link into the LinkedIn post** (first comment, not the body — LinkedIn deprioritizes posts with external links).

**Pros:** Real-looking, version-controllable, others can contribute via PRs, the skill format is correct for Claude Code users.
**Cons:** Some people see GitHub and bounce. Not all your LinkedIn audience is technical.

---

## Path B: Google Drive folder (easiest, lowest-friction)

**Audience:** Non-technical LinkedIn folks who want to copy-paste a prompt into ChatGPT/Claude.

**Steps:**

1. **Create a new folder in your Google Drive:** "Career Search Coach — Free Tool"

2. **Upload the files** by uploading these:
   - README.md (convert to Google Doc on upload)
   - STANDALONE_PROMPT.md (convert to Google Doc)
   - Optionally: zip the `skill/` folder and upload as one file

3. **Set folder sharing:** Right-click the folder → Share → "Anyone with the link" → Viewer

4. **Copy the folder share link.**

5. **In the LinkedIn post first comment, link to the folder.**

**Pros:** Familiar interface for non-technical audience. Zero friction to use the standalone prompt.
**Cons:** Doesn't feel as "official." Hard to version-update. Doesn't work as an installable Claude Code skill cleanly.

---

## Path C: Both (recommended for maximum reach)

Do Path A AND Path B:

- GitHub repo for the technical audience + future contributors
- Google Doc with the STANDALONE_PROMPT for one-click copy-paste

In the LinkedIn post comment, link to both:
> 🔧 Standalone prompt (use with Claude.ai, no install): [Google Doc link]
> 💻 Full skill + reference docs (Claude Code or contribute): [GitHub link]

---

## Optional Path D: A Notion page (middle ground)

If you have a Notion account and prefer that aesthetic:

1. Create a public Notion page titled "Career Search Coach"
2. Paste the README.md content as the cover/intro
3. Embed the STANDALONE_PROMPT.md content as a copyable code block
4. Link references docs as subpages
5. Publish to web → copy the public URL

**Pros:** Pretty layout, easy edits, copyable code blocks built-in.
**Cons:** Requires Notion account for you (not the user). Less version-friendly.

---

## After publishing — what to do

1. **Post on LinkedIn** using one of the post drafts in `LINKEDIN_POST.md`
2. **Pin the post** to your profile for 2–4 weeks
3. **Reply to comments quickly** — first 1–2 hours determines reach
4. **Tag 2–3 friends** in transition in the comments — multiplies signal
5. **One week later:** post an update — "X people have used it, here's what I'm hearing" — drives a second wave
6. **Add a featured section** to your LinkedIn profile linking to the tool
7. **Consider cross-posting** to Twitter/X with a tighter version of Version C

---

## Maintenance

You don't need to actively maintain this once it's published. But every few weeks, consider:

- **Reviewing the SKILL.md and references for accuracy** — your own search will surface gaps
- **Adding a CHANGELOG.md** if you make updates
- **Responding to GitHub issues** if anyone files one

The goal isn't to build a product. It's to share a tool, help others, and keep the karma loop going.

---

## What this gives you (personally)

Beyond helping others, publishing this:

1. **Builds your own credibility** as someone who systematizes complex problems
2. **Surfaces opportunities** — people will message you about other things
3. **Documents the playbook** for your own future searches
4. **Signals "thoughtful operator"** to anyone evaluating you for senior roles

The post itself is a brand-building artifact. Treat it like one.

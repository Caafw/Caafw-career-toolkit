# CAAFW Career Toolkit Skill
## Pit Stop — Career Toolkit by caafw.org

**Version:** 1.0.0  
**Author:** Ajay Sharma FCIPD · CIPD UK AI Advisory Board  
**Website:** [caafw.org](https://caafw.org) · [caafw.org/join](https://caafw.org/join)  
**GitHub:** [github.com/caafw-org/career-toolkit](https://github.com/caafw-org/career-toolkit)  
**Licence:** MIT — free to use, share, and build on

---

## What This Skill Does

Install this skill into Claude once. Then type `/career-toolkit` — Claude will ask for your CV and a few details, then generate a complete, personalised career plan as a polished HTML file you can open in any browser, share, or print.

**Output includes:**
- Rewritten profile & 60-second elevator pitch
- Three LinkedIn headline options
- Target companies with fit scores (★ Strong / ✓ Good / ◆ Stretch)
- Five copy-paste outreach templates (LinkedIn, email, follow-up, recruiter, reconnect)
- Situation-specific guidance (career break / visa / senior transition / graduate)
- 90-day action plan with salary benchmarks

**It uses your own Claude account and your own API credits. CAAFW does not collect your data.**

---

## Install in 3 Steps

### Step 1 — Download this file
Save `SKILL.md` to your computer.

### Step 2 — Install on Claude.ai (free, 2 minutes)
1. Go to **[claude.ai](https://claude.ai)** — sign in (free account works)
2. Click **Projects** in the left sidebar
3. Click **New Project** — name it "Career Toolkit"
4. Click **Add instructions** (or "Project instructions")
5. Open this `SKILL.md` file, copy all the text, paste it in
6. Click **Save**

### Step 3 — Use it
Start a new chat inside your Career Toolkit project.  
Attach your CV file (or paste the text), then type:

```
/career-toolkit
```

Claude will ask for your situation, target market, and sector — then generate your personalised toolkit in under 60 seconds.

---

## Commands

| Command | What You Get |
|---------|-------------|
| `/career-toolkit` | Full interactive HTML toolkit — all 6 tabs |
| `/career-pitch` | Elevator pitch + 3 LinkedIn headlines only |
| `/career-targets` | 10 target companies with fit scores |
| `/career-messages` | 3 outreach templates |
| `/career-plan` | 90-day action plan |
| `/career-help` | Show all commands |

---

## How Claude Should Behave (Skill Instructions)

When the user types `/career-toolkit` or shares their CV, follow these instructions precisely.

### Step 1 — Gather Information

Ask all of the following in a single message if not already provided:

```
To build your personalised career toolkit, I need a few details:

1. Your CV — paste the full text below (or attach the file)
2. Your situation:
   - 🎓 Final year student / recent graduate
   - 🔄 Career transition (moving sector or role type)
   - ⏸️ Returning from career break (maternity, family, personal)
   - 📈 Senior professional (targeting Director / VP / C-suite)
   - ✈️ International professional (visa constraints apply)
   - 🚀 Active job search (currently looking)
3. Target market — e.g. London, New York, Manila, US nationwide
4. Target sector — e.g. Tech/AI, Finance, HR, Open to all
5. Target role — e.g. Data Scientist, Head of HR (or "recommend best fit")
6. Work authorisation — e.g. UK citizen, F-1 OPT, Skilled Worker Visa
7. Career breaks? Yes/No, brief description if yes
```

### Step 2 — Generate the HTML Toolkit

Once you have the CV and context, generate a **complete, single-file HTML** following this specification.

---

## HTML Output Specification

### Design
- **Background:** Pure black `#000000`
- **Text:** Pure white `#ffffff`
- **Cards/panels:** `#111111` with `1px solid #333333` borders
- **Buttons:** White background `#ffffff`, black text `#000000`
- **Typography:** EB Garamond (serif, headings) + Manrope (sans, body) — Google Fonts
- **No colour other than black and white**

### Required Tabs (6)

**Tab 1 — Profile & Pitch**
- Readiness score (0–100) with label and one-line note
- Rewritten CV summary (2–3 paragraphs, specific to their background)
- 3 LinkedIn headline options
- 60-second elevator pitch (first person, copy button)
- 2×2 strengths grid with evidence from their actual CV
- One honest observation about what most needs fixing

**Tab 2 — Target Roles & Companies**
- Best-fit role titles (4–5) with brief rationale
- Company table: minimum 8 **real, named** companies with: Company · Role · Why it fits · Fit rating
- Salary benchmarks for their level and market (real ranges, not "varies")

**Tab 3 — How to Search**
- 6-step numbered process with bold titles and readable body text
- 2 copy-paste LinkedIn search strings (sector-specific)
- Job boards specific to their market (not generic global list)
- Visa/authorisation guidance if applicable
- One search strategy insight specific to their situation

**Tab 4 — Message Templates**
Five templates, each with one-click copy button and character count:
1. LinkedIn connection request (under 280 chars, warm and specific)
2. Cold email application (subject + 3 paragraphs + sign-off)
3. Follow-up message (5 days after, under 150 words)
4. Recruiter/agency outreach (email format)
5. Former colleague reconnect (LinkedIn/WhatsApp format)

**Tab 5 — Situation-Specific**
Title and content based on their situation:
- Graduate → `Graduate Job Search Strategy` (OPT/visa, alumni network, first role tips)
- Transition → `Transition Strategy & Reframing Narrative` (transferable skills, first move)
- Break → `Addressing the Career Gap` (interview answers, CV formatting, returnships)
- Senior → `Executive Positioning & Search Strategy` (search firms, leadership narrative)
- International → `Visa Pathway & Market Entry` (sponsor-friendly employers, visa timeline)
- Active → `Accelerated Search Strategy` (sharpen targeting, outreach volume, weekly plan)

**Tab 6 — 90-Day Plan**
- 4 milestones: Week 1–2 (Foundation) · Month 1 (Activate) · Month 2 (Apply) · Month 3 (Convert)
- Weekly rhythm (Mon–Fri, specific daily actions)
- Salary benchmarks
- One honest risk observation

### Required Footer (on every page)
```html
<footer>
  <p>Career Toolkit — Pit Stop by CAAFW &nbsp;·&nbsp;
     <a href="https://caafw.org/join">caafw.org/join</a> &nbsp;·&nbsp;
     Centre for Applied AI and Future of Work
  </p>
  <p>Check your AI Readiness: 
     <a href="https://www.caafw.org/Readiness">www.caafw.org/Readiness</a> &nbsp;·&nbsp;
     © 2026 www.caafw.org
  </p>
</footer>
```

### Technical Requirements
- Single self-contained `.html` file — all CSS and JS inline, no external dependencies except Google Fonts
- All message templates have `onclick` copy-to-clipboard buttons
- Mobile responsive (works at 375px)
- Smooth tab transitions
- Works offline after first load
- Background forced black on all elements (use `background:#000000 !important` on html, body, and all panels)

---

## Quality Standards

**Be specific, never generic:**
- ✅ "Apply to Mishcon de Reya, Fieldfisher, and Eversheds for ER Manager roles"
- ❌ "Apply to law firms in London"

**Salary benchmarks must be real ranges:**
- ✅ "Senior HR Manager in London: £55,000–£72,000"
- ❌ "Salary varies by company"

**Companies must be real and named:**
- Use actual organisations appropriate to their sector and market
- Include a mix of large and boutique/specialist firms
- Mark stretch companies honestly

**Address breaks and visas directly:**
- Name the break, own it, pivot to strengths
- Never suggest fabricated freelance work

---

## Quick Commands

### `/career-pitch`
Ask for CV only. Respond in plain text:
1. 60-second elevator pitch (first person)
2. Three LinkedIn headline options
3. Top three strengths with CV evidence

### `/career-targets`
Ask for CV + sector + market. Return a formatted table of 10 companies.

### `/career-messages`
Ask for CV + situation + target role. Generate 3 templates.

### `/career-plan`
Ask for situation + timeline. Generate 90-day plan as numbered milestones.

### `/career-help`
Print the command table above and a brief description.

---

## About CAAFW

**Centre for Applied AI and Future of Work**  
Six pillars: Discover · Re/Skill · Experiment · Stride · Work · Marketplace

This skill is part of CAAFW's commitment to making AI-powered career guidance free and accessible to everyone. It runs entirely on your own Claude account — CAAFW does not see your CV, your data, or your outputs.

→ **Join the community:** [caafw.org/join](https://caafw.org/join)  
→ **Check your AI Readiness:** [www.caafw.org/Readiness](https://www.caafw.org/Readiness)

---

*Fork it. Translate it. Improve it. That's the point.*

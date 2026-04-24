# CAAFW Career Toolkit
## Pit Stop — AI-Powered Career Planning · Free · Open Source

[![Licence: MIT](https://img.shields.io/badge/Licence-MIT-white.svg)](LICENSE)
[![Made with Claude](https://img.shields.io/badge/Powered%20by-Claude%20AI-black.svg)](https://claude.ai)
[![CAAFW](https://img.shields.io/badge/Built%20by-CAAFW-black.svg)](https://caafw.org)

**Turn your CV into a complete career plan in 60 seconds.**  
Install once on Claude. Type one command. Get your pitch, target companies, outreach messages, and a 90-day plan — personalised to your actual CV.

→ **[See a live sample](https://caafw.org/toolkit)** · **[Join CAAFW](https://caafw.org/join)**

---

## How It Works

```
Your CV  +  /career-toolkit  =  Full personalised HTML career plan
```

1. **Download** `SKILL.md` from this repo
2. **Install** it into Claude.ai (free account, 2 minutes)
3. **Paste your CV** and type `/career-toolkit`
4. **Receive** a complete career toolkit as a downloadable HTML file

**Your CV stays on your device. CAAFW never sees your data. You use your own Claude credits.**

---

## What the Toolkit Contains

| Tab | What's Inside |
|-----|--------------|
| **Profile & Pitch** | Rewritten CV summary · Readiness score · 3 LinkedIn headlines · 60-second pitch · Strengths grid |
| **Target Companies** | 8+ real named companies · Fit scores · Role recommendations · Salary benchmarks |
| **How to Search** | Step-by-step process · LinkedIn search strings · Job boards for your market · Visa guidance |
| **Message Templates** | LinkedIn note · Cold email · Follow-up · Recruiter outreach · Colleague reconnect — all copy-paste ready |
| **Situation Guide** | Career break / Graduate / Senior / Visa / Transition — specific to your situation |
| **90-Day Plan** | Week-by-week milestones · Daily rhythm · Salary ranges · Honest risk assessment |

---

## Install in 3 Steps

### Step 1 — Get the Skill File

**Option A — Download directly:**  
Click `SKILL.md` above → Raw → Save as `SKILL.md`

**Option B — Clone the repo:**
```bash
git clone https://github.com/caafw-org/career-toolkit.git
```

---

### Step 2 — Install on Claude.ai

1. Go to **[claude.ai](https://claude.ai)** (free account works)
2. Click **Projects** in the left sidebar
3. **New Project** → name it "Career Toolkit"
4. Click **Add instructions**
5. Open `SKILL.md`, copy all content, paste it in → **Save**

> One install. Works forever. Every conversation in the project has the skill active.

---

### Step 3 — Generate Your Toolkit

Start a new chat in your Career Toolkit project.  
Paste your CV text (or attach the file), then type:

```
/career-toolkit
```

Claude asks a few quick questions then generates your personalised HTML file.

---

## All Commands

| Command | Output |
|---------|--------|
| `/career-toolkit` | **Full toolkit** — complete interactive HTML, all 6 tabs |
| `/career-pitch` | Elevator pitch + 3 LinkedIn headlines |
| `/career-targets` | 10 target companies with fit scores |
| `/career-messages` | 3 outreach templates |
| `/career-plan` | 90-day action plan |
| `/career-help` | Show all commands |

---

## Supported Situations

| Situation | What Claude focuses on |
|-----------|----------------------|
| 🎓 Graduate / Final year | First role, OPT/visa, alumni network |
| 🔄 Career transition | Transferable skills, reframing narrative |
| ⏸️ Returning from break | Addressing the gap, returnships, interview answers |
| 📈 Senior professional | Executive search, leadership narrative, C-suite targeting |
| ✈️ International / Visa | Sponsor-friendly employers, visa pathway, market entry |
| 🚀 Active job search | Sharpened targeting, outreach volume, weekly rhythm |

## Supported Markets

UK · United States · India · Philippines · Singapore · UAE · Remote / Global

---

## Sample Output

A live sample toolkit (fictional profile: Riya Kapoor, Data Analyst → Product Manager, London) is hosted at **[caafw.org/toolkit](https://caafw.org/toolkit)**

The sample shows exactly what the skill generates — so you know what you're getting before you install.

---

## Using the API Instead

If you're a developer and want to call Claude directly:

```python
import anthropic

with open('SKILL.md', 'r') as f:
    skill = f.read()

client = anthropic.Anthropic()

response = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=8000,
    system=skill,
    messages=[{
        "role": "user",
        "content": "/career-toolkit\n\n[Paste CV text here]"
    }]
)

print(response.content[0].text)
```

---

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

**Priority contributions needed:**
- New markets (Singapore, UAE, Germany, Canada, Australia)
- New situations (PhD to industry, military to civilian, nonprofit to corporate)
- Translations (Hindi, Filipino, Spanish, Arabic)
- Output quality improvements for specific sectors

---

## Licence

MIT — free to use, share, modify, and build on.

Attribution appreciated: *"Powered by CAAFW · caafw.org/join"*

---

## About CAAFW

**Centre for Applied AI and Future of Work**

CAAFW helps professionals, SMBs, and students across the UK, US, India, and the Philippines adopt AI practically and responsibly.

Six pillars: **Discover · Re/Skill · Experiment · Stride · Work · Marketplace**

- 🌐 [caafw.org](https://caafw.org)
- 🚀 [caafw.org/join](https://caafw.org/join) — Join the community
- 📊 [www.caafw.org/Readiness](https://www.caafw.org/Readiness) — AI Readiness assessment

Built by **Ajay Sharma FCIPD** — CIPD UK AI Advisory Board · Visiting Faculty, University of Liverpool · Carnegie Mellon AI Certified

---

*If this toolkit helped you land a role, change direction, or build confidence — we'd love to hear about it.*  
*Share your story: [caafw.org/join](https://caafw.org/join)*

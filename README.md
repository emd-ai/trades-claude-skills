# Claude Skills for Trades & Services Businesses

10 ready-to-use AI skills that any local trades business — HVAC, electrical, plumbing, roofing — can install in under 5 minutes.

No coding. No technical background. These are not demos — they solve real problems that cost trades businesses money every day.

---

## How Skills Work

A Claude Skill is not a full app or integration. It's a reusable workflow that tells Claude how to handle a repeat business task. You run the skill, give it the job details, and Claude drafts the estimate, follow-up, response, or campaign for you.

Think of it like a really good employee who already knows your format, your rates, and your voice — and can produce a finished document in 30 seconds instead of 30 minutes.

**Skills are:**
- Plain-English instructions — no code, no API, no setup
- Saved once, reused every time
- Private to your account

**Skills are NOT:**
- A CRM or scheduling tool
- Connected to your phone or email (you copy-paste the output)
- A replacement for field work — they handle the paperwork side

---

## What Happens When I Use One?

```
1. Type the skill command         →  /estimate-writer
2. Paste the job details          →  "Quote for Tom at 88 River Rd, panel upgrade..."
3. Claude generates the output    →  Formatted estimate + follow-up messages
4. You send it                    →  Copy into email, iMessage, or your CRM
```

That's it. Every skill follows this pattern — you provide the details, Claude produces the document, you use it.

---

## Manual vs Automated

There are two ways to use these skills, depending on your comfort level:

| | Claude.ai (browser) | Claude Code (terminal) |
|---|---|---|
| **How it works** | Open claude.ai, type the command, paste details, get output | Run from the command line alongside your code or scripts |
| **Who it's for** | Business owners, office staff, techs on their phone | Developers, tech-savvy owners, service providers |
| **Automation** | Manual — you run each skill by hand | Can be scripted, scheduled, or chained together |
| **Setup** | Upload a ZIP file — 2 minutes | Clone the repo — 5 minutes |

**Most trades business owners should use Claude.ai.** It's the simplest path — no terminal, no coding. Claude Code is for service providers who deliver these skills on behalf of clients or want to automate workflows.

---

## Install

### Option A — Claude.ai (recommended for most users)

No terminal. No coding. Works in your browser.

**Requires:** A Claude Pro, Max, Team, or Enterprise subscription

1. Download the skills ZIP file: [**trades-claude-skills.zip**](https://github.com/emd-ai/trades-claude-skills/releases/download/v1.0.0/trades-claude-skills.zip)
2. Go to [claude.ai](https://claude.ai) → click your profile icon → **Settings**
3. Click **Customize**
4. Scroll to the **Skills** section → click **Upload skill**
5. Upload the ZIP file
6. Your skills appear in the list — toggle each one on

That's it. Open a new chat and type `/estimate-writer` (or any skill command) to use it.

**Note:** Skills are private to your account. If you have a team, each person uploads the ZIP separately.

#### What's inside the ZIP?

```
trades-claude-skills/
└── skills/
    ├── estimate-writer/
    │   └── SKILL.md          ← instructions for this skill
    ├── job-proposal-writer/
    │   └── SKILL.md
    ├── review-responder/
    │   └── SKILL.md
    └── ... (10 skill folders total)
```

Each skill is a folder containing one file — `SKILL.md`. That file is the entire skill. Claude reads it and knows what to do. There's no hidden complexity.

**Troubleshooting:** If the upload doesn't work, make sure the ZIP contains the `skills/` folder at the root level (not nested inside another folder). Some systems create an extra wrapper folder when you download from GitHub — if you see `trades-claude-skills-main/skills/`, rename the outer folder or re-zip just the `skills/` directory.

---

### Option B — Claude Code (for developers)

Command-line tool. More control. Required for automating workflows.

**Requires:** Node.js 18+ ([download here](https://nodejs.org))

```bash
# Install Claude Code
npm install -g @anthropic/claude-code

# Clone this repo
git clone https://github.com/emd-ai/trades-claude-skills.git

# Copy skills into your project
cp -r trades-claude-skills/skills/ .claude/skills/

# Launch
claude
```

Skills are auto-discovered. Type any skill command to use it.

---

## The 10 Skills

### Core Operations

| Skill | What it does | Time saved |
|-------|-------------|-----------|
| [`/estimate-writer`](#1-estimate-writer) | Professional quote in 2 minutes | 30–90 min/quote |
| [`/job-proposal-writer`](#2-job-proposal-writer) | Multi-page competitive bid for $5K+ jobs | 2–3 hours/proposal |
| [`/service-agreement-writer`](#3-service-agreement-writer) | Recurring maintenance plans that build revenue | 3–4 hours/agreement |
| [`/lien-waiver-generator`](#4-lien-waiver-generator) | Correct lien waiver for any payment situation | 30–60 min/waiver |
| [`/hiring-post-writer`](#5-hiring-post-writer) | Job listing that actually attracts applicants | 1–2 hours/post |

### Customer Communication

| Skill | What it does | Time saved |
|-------|-------------|-----------|
| [`/job-complete-followup`](#6-job-complete-followup) | Review request + re-engagement after every job | 10 min/job |
| [`/review-responder`](#7-review-responder) | Google review responses that help your ranking | 5–15 min/review |
| [`/missed-call-handler`](#8-missed-call-handler) | Immediate SMS recovery for missed calls | Every missed lead |
| [`/seasonal-campaign`](#9-seasonal-campaign) | Past customer campaigns timed to your seasons | 4–8 hours/campaign |
| [`/complaint-resolution-writer`](#10-complaint-resolution-writer) | Professional dispute resolution + documentation | 1–3 hours/complaint |

---

## How to use each skill

---

### 1. Estimate Writer

**The problem it solves:** Writing quotes takes 30–90 minutes per job. Half of them never get replied to anyway because the follow-up falls through.

**Use it like this:**

```
/estimate-writer

Customer: Tom Bradley, 88 River Road
Job: Full rewire, 3-bed house
Labour: 3 days, 2 electricians at $85/hr each
Materials: ~$1,200 cable, boards, fittings
Call-out: $75
Terms: 40% upfront, balance on completion
My licence: EC-12345
```

**What you get back:**

- Complete formatted estimate document (copy into Word/Google Docs, save as PDF)
- Text message to send with the estimate
- Day 3 follow-up message (if no response)
- Day 7 final follow-up message

**Tip:** First time you use it, tell Claude your standard labour rate, payment terms, and warranty. It applies them to every estimate automatically.

---

### 2. Job Proposal Writer

**The problem it solves:** For jobs over $5K, a one-page estimate won't win competitive bids. You need a document that sells your company, not just your price. Contractors who send professional proposals close 25–35% more large jobs.

**Use it like this:**

```
/job-proposal-writer

Customer: Sarah at 15 Elm Court
Job: Full HVAC replacement — old R-22 system to new 16 SEER2
Price: $12,800 standard, $16,500 for high-efficiency 20 SEER2
Timeline: 2 days
Financing: 0% for 18 months
We've been in business 14 years, fully licenced and insured.
```

**What you get back:**

- Cover letter that leads with the customer's problem
- Detailed scope of work (inclusions, exclusions, deliverables)
- Three pricing options (Good / Better / Best) — customers choose the middle 60% of the time
- Project timeline with milestones
- Company credentials section
- Payment schedule with financing options
- Follow-up sequence (Day 3, Day 7, Day 14)

**When to use this vs. estimate-writer:** Estimates are 1-page price quotes for straightforward jobs. Proposals are 3–5 page persuasive documents for competitive bids over $5K.

---

### 3. Service Agreement Writer

**The problem it solves:** Maintenance agreements are 55% of trades industry revenue. They turn one-time customers into recurring revenue — no more feast-or-famine seasonal swings. Most small operators don't offer them because they don't know how to write one.

**Use it like this:**

```
/service-agreement-writer

Trade: HVAC
Visits: 1 for Bronze, 2 for Silver, 4 for Gold
Pricing: $179/yr, $299/yr, $449/yr
Parts discount: 10% Bronze, 15% Silver, 20% Gold
Priority scheduling for Silver and Gold
Same-day emergency response for Gold only
```

**What you get back:**

- Complete tiered agreement document (Bronze / Silver / Gold)
- Trade-specific visit checklist (what gets inspected/serviced)
- Sales script for technicians to pitch on-site after a job
- Email template to send the agreement
- Follow-up message (7 days)
- Renewal reminder (30 days before expiry)

**Industry target:** 250 service agreements per $1M in annual revenue.

---

### 4. Lien Waiver Generator

**The problem it solves:** Lien waivers are required on every commercial project payment. Wrong waiver type = delayed cash flow or lost lien rights. This skill asks two questions and produces the correct waiver every time.

**Use it like this:**

```
/lien-waiver-generator

Project: Thompson Office Renovation at 500 Main Street
Owner: Thompson Properties LLC
GC: ABC General Contractors hired me
Payment: $8,500 for work through March 15th
Haven't been paid yet
There's a $1,200 change order still being negotiated
```

**What you get back:**

- The correct waiver type (Conditional Progress in this case)
- Completed waiver document with all fields filled
- Change order listed as an exception (protecting your rights)
- Warning: don't sign the unconditional version until payment clears
- Project waiver tracker template

**The 4 types:** Conditional Progress, Unconditional Progress, Conditional Final, Unconditional Final — the skill picks the right one based on your situation.

---

### 5. Hiring Post Writer

**The problem it solves:** 110,000+ technician shortage in HVAC alone. Every trade is facing the same crisis. If your job listing says "Hiring HVAC tech. Call us." — that's why nobody's applying. Job posts with specific pay ranges get 2–3x more applicants.

**Use it like this:**

```
/hiring-post-writer

Role: Residential HVAC service technician
Location: Phoenix
Experience: 2+ years, EPA 608 required
Pay: $28–36/hr
Benefits: Health insurance, company van, gas card,
$500/yr tool allowance, paid continuing education
We're a 14-year-old family business, crew of 8
Referral bonus: $500
```

**What you get back:**

- Full job listing for Indeed / ZipRecruiter (professional, specific, sells the job)
- Social media version for Facebook / Instagram / Nextdoor
- Referral bonus flyer (print or text to your crew)
- 5 tailored interview questions

**Apprentice mode:** Tell it you're hiring an apprentice and it removes experience requirements, emphasises training and career path.

---

### 6. Job Complete Followup

**The problem it solves:** You finish a job, get in the van, and forget to follow up. The customer forgets to leave a review. The relationship ends there.

**Use it like this:**

```
/job-complete-followup

Just finished installing a new water heater for Mike at
234 Oak Street. My tech was Dave. Mike was really pleased
— said it was the best service he'd had. My Google review
link is g.page/r/[your-link]/review
```

**What you get back:**

- SMS review request (under 160 chars, ready to send)
- Email version if you prefer
- 90-day re-engagement message (put it in your calendar)
- CRM log entry

**Real example output:**

> Hi Mike, it's Dave from [Business]! Really glad the new water heater is sorted. If you have 60 seconds, a Google review would mean everything to us: [link]. Thanks so much!

---

### 7. Review Responder

**The problem it solves:** 60–80% of reviews on the average trades business profile have no response. Google treats this as a signal that the business is inactive. Your competitors who respond climb above you in local search.

**Use it like this — just paste the review:**

```
/review-responder

"Arrived on time, very professional. Fixed our boiler quickly
and explained everything. Will definitely use again. 5 stars."
```

**What you get back:**

A ready-to-post response, under 150 words, that:
- References the specific job
- Includes your city name naturally (local SEO)
- Sounds like you wrote it, not a template

**For negative reviews:**

```
/review-responder

"They no-showed for the first appointment and didn't call.
Had to take a day off work. Very disappointed."
```

Claude handles these carefully — acknowledges the issue, doesn't argue, offers offline resolution, never makes excuses publicly.

**Volume tip:** If you have 20 unanswered reviews sitting there right now, paste them all at once numbered 1–20. Get them all responded to in one session.

---

### 8. Missed Call Handler

**The problem it solves:** A homeowner calls three companies. The one who responds first gets the job. Most trades businesses see the missed call an hour later and either don't call back or call back cold with no context.

**Use it like this:**

```
/missed-call-handler

Missed call from unknown number at 5:45pm. I'm an HVAC tech,
business name is Arctic Air, I'm based in Phoenix.
```

**What you get back — send within 5 minutes:**

> Hi, this is Mike from Arctic Air. Sorry I missed your call — I was finishing up a job. What can I help you with? Happy to call you back in 15 minutes or answer over text.

**For after-hours calls:**

```
/missed-call-handler

Missed call at 9pm from a number I don't recognise.
Do handle emergency call-outs.
```

Claude produces an urgent-appropriate response that signals you take emergency work seriously.

---

### 9. Seasonal Campaign

**The problem it solves:** Your past customers are your cheapest source of new revenue. They already trust you. Most trades businesses contact them zero times per year unless they call in.

**Use it like this:**

```
/seasonal-campaign

Trade: HVAC
Campaign: Pre-summer AC tune-up
Customers: Everyone who had AC work done in the last 2 years (~60 customers)
Offer: $30 off tune-up booked before May 1st
My slots: Can take 20 more tune-ups this spring
```

**What you get back:**

A complete 3-touch campaign:
- Touch 1: SMS + email (Week 1)
- Touch 2: Nudge to non-responders (Day 10)
- Touch 3: Final call (Day 17)

Plus a referral add-on line to include in Touch 1 for happy past customers.

**What "good" looks like for 60 customers:**
- 8–15% booking rate = 5–9 booked jobs
- 1–3 referrals from enthusiastic responders
- Zero ad spend

---

### 10. Complaint Resolution Writer

**The problem it solves:** Customer complaints — billing disputes, warranty claims, BBB complaints, angry emails — are the tasks that keep business owners up at night. An unresolved complaint costs you 10+ referrals. A well-handled one can become your most loyal customer.

**Use it like this:**

```
/complaint-resolution-writer

Customer: John at 45 Oak Street
Complaint: Says the new AC unit we installed is making a rattling noise
and we haven't responded to his calls for 3 days.
Our side: Tech was sick, office missed the callback. Unit is installed
correctly but may need a mounting bracket adjustment.
Willing to offer: Free callback visit this week to inspect and fix.
```

**What you get back:**

- Professional response letter (acknowledges issue, provides timeline, offers resolution)
- Internal incident log (protects you if it escalates)
- Follow-up message after resolution
- BBB response format (if applicable)
- Escalation letter (if they reject your offer)

**Different from review-responder:** Review-responder handles public Google/Yelp reviews (short, SEO-focused). This handles private disputes (detailed, factual, protective).

---

## Customising for your trade

These skills work for any trades or services business. Here's how each maps:

| Trade | Best starting skills | Why |
|-------|-------------------|-----|
| HVAC | `/seasonal-campaign` + `/service-agreement-writer` | Seasonal demand + recurring revenue |
| Electrician | `/estimate-writer` + `/job-proposal-writer` | Quotes and competitive bids |
| Plumber | `/missed-call-handler` + `/complaint-resolution-writer` | Emergency response + dispute handling |
| Roofer | `/review-responder` + `/lien-waiver-generator` | Search-driven + commercial payment docs |
| Landscaper | `/job-complete-followup` + `/service-agreement-writer` | Repeat business + maintenance plans |
| Painter | `/estimate-writer` + `/hiring-post-writer` | Pipeline + labour shortage |
| General Contractor | `/job-proposal-writer` + `/lien-waiver-generator` | Competitive bids + payment paperwork |

---

## Building your own skills

These 10 are a starting point. Every business has workflows that are unique to them.

**To build your own skill:**

1. Create a new folder in `.claude/skills/your-skill-name/`
2. Create `SKILL.md` inside it
3. At the top, add a description block:

```markdown
---
name: your-skill-name
description: Use this skill when [specific trigger].
             Triggers on phrases like [examples].
             Do NOT use for [what it's not for].
---
```

4. Then write exactly what you want Claude to do — in plain English. No code needed.

**Ideas for trades-specific skills to build next:**

- `/scope-of-work-generator` — detailed SOW documents from a brief job description
- `/change-order-writer` — formal change orders with cost adjustments mid-project
- `/end-of-day-report` — structured daily reports from quick voice notes or bullet points
- `/safety-toolbox-talk` — OSHA-aligned daily/weekly safety meeting briefs
- `/invoice-chaser` — polite payment follow-up sequence for overdue invoices
- `/subcontractor-brief` — brief out work to a subie with your standards embedded

---

## For service providers — done-for-you delivery

If you deliver these skills on behalf of clients (as part of a setup service, onboarding package, or managed offering), the `/templates/` and `/linkedin-skills/` folders automate the entire build process.

### How it works

1. **Collect the intake form** — 15 required fields + 2 optional from your client (business name, owner, city, services, rates, terms, etc.)
2. **Run `/client-build`** — reads the 10 templates, substitutes all `{{PLACEHOLDER}}` variables with the client's data in one pass, validates completeness
3. **Run `/reference-card`** — generates a one-page quick reference the client can print or keep on their phone
4. **Deliver** — zip `/clients/[business-name]/` and send with upload instructions for claude.ai

Client builds go into `/clients/` which is gitignored — no client data ever touches the public repo.

### What's in `/templates/`

Template versions of all 10 skills using `{{DOUBLE_CURLY_BRACE}}` placeholders for automated find-and-replace. Single-bracket `[items]` are runtime inputs the client fills in per use — those stay as-is.

### Operational skills

| Skill | What it does |
|-------|-------------|
| `/linkedin-skills/client-build/` | Builds all 10 skills from an intake form → ready-to-zip client folder |
| `/linkedin-skills/reference-card/` | Generates the client's one-page delivery document |

---

## Who built this

Built by Eoin Michael McDonnell — founder of HVACRanker, a platform that automates reviews, reputation management, and customer re-engagement for HVAC businesses.

If you run an HVAC business specifically and want this fully automated — review requests, AI-drafted responses, seasonal campaigns — without doing any of it manually, that's what HVACRanker does.

[→ hvacranker.io](https://hvacranker.io)

---

## Contributing

If you build a skill that works well for your trade, open a PR. The goal is a library of skills covering every common workflow in trades and services — built by the people who actually do the work.

---

## Licence

MIT — use it, modify it, share it. No strings.

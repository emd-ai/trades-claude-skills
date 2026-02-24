# Claude Skills for Trades & Services Businesses

5 ready-to-use AI skills that any local trades business — HVAC, electrical, plumbing, roofing — can install in under 5 minutes.

No coding. No technical background. These are not demos — they solve real problems that cost trades businesses money every day.

---

## What are Claude Skills?

A Claude Skill is a set of instructions that tells Claude exactly how to handle a specific task in your business. You install it once. After that, you type a short command and Claude does the work.

Works in the Claude app (browser) or Claude Code (terminal).

---

## Two ways to install

### Option A — Claude.ai (recommended for most users)

No terminal. No coding. Works in your browser.

**Requires:** A Claude Pro, Max, Team, or Enterprise subscription

1. Download the skills ZIP file: [**trades-claude-skills.zip**](https://github.com/emd-ai/trades-claude-skills/releases/download/v1.0.0/trades-claude-skills.zip)
2. Go to [claude.ai](https://claude.ai) → click your profile icon → **Settings**
3. Click **Capabilities**
4. Make sure **Code execution and file creation** is toggled ON
5. Scroll to the **Skills** section → click **Upload skill**
6. Upload the ZIP file
7. Your skills appear in the list — toggle each one on

That's it. Open a new chat and type `/job-complete-followup` (or any skill command) to use it.

**Note:** Skills are private to your account. If you have a team, each person uploads the ZIP separately.

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

## The 5 Skills

| Skill | What it does | Time saved |
|-------|-------------|-----------|
| [`/job-complete-followup`](#1-job-complete-followup) | Review request + re-engagement after every job | 10 min/job |
| [`/estimate-writer`](#2-estimate-writer) | Professional quote in 2 minutes | 30–90 min/quote |
| [`/review-responder`](#3-review-responder) | Google review responses that help your ranking | 5–15 min/review |
| [`/missed-call-handler`](#4-missed-call-handler) | Immediate SMS recovery for missed calls | Every missed lead |
| [`/seasonal-campaign`](#5-seasonal-campaign) | Past customer campaigns timed to your seasons | 4–8 hours/campaign |

---

## How to use each skill

---

### 1. Job Complete Followup

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

### 2. Estimate Writer

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

### 3. Review Responder

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

### 4. Missed Call Handler

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

### 5. Seasonal Campaign

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

## Customising for your trade

These skills work for any trades or services business. Here's how each maps:

| Trade | Best starting skill | Why |
|-------|-------------------|-----|
| HVAC | `/seasonal-campaign` | Highest ROI — massive seasonal demand cycles |
| Electrician | `/estimate-writer` | Quotes take the most time, lose the most leads |
| Plumber | `/missed-call-handler` | Emergency nature means response speed = everything |
| Roofer | `/review-responder` | Most search-driven trade — reviews matter most |
| Landscaper | `/job-complete-followup` | Repeat and referral business is the whole model |
| Painter | `/estimate-writer` + `/job-complete-followup` | Quotes + referrals are the whole pipeline |

---

## Building your own skills

These 5 are a starting point. Every business has workflows that are unique to them.

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

- `/warranty-claim-handler` — triage incoming warranty calls, produce response + schedule
- `/subcontractor-brief` — brief out work to a subie with your standards embedded
- `/material-order` — generate a materials list from a job description
- `/job-debrief` — end of day notes, photo checklist, anything to capture for the job file
- `/complaint-handler` — structured response to complaints before they hit Google
- `/invoice-chaser` — polite payment follow-up sequence for overdue invoices

---

## For service providers — done-for-you delivery

If you deliver these skills on behalf of clients (as part of a setup service, onboarding package, or managed offering), the `/templates/` and `/linkedin-skills/` folders automate the entire build process.

### How it works

1. **Collect the intake form** — 15 required fields + 2 optional from your client (business name, owner, city, services, rates, terms, etc.)
2. **Run `/client-build`** — reads the 5 templates, substitutes all `{{PLACEHOLDER}}` variables with the client's data in one pass, validates completeness
3. **Run `/reference-card`** — generates a one-page quick reference the client can print or keep on their phone
4. **Deliver** — zip `/clients/[business-name]/` and send with upload instructions for claude.ai

Client builds go into `/clients/` which is gitignored — no client data ever touches the public repo.

### What's in `/templates/`

Template versions of all 5 skills using `{{DOUBLE_CURLY_BRACE}}` placeholders for automated find-and-replace. Single-bracket `[items]` are runtime inputs the client fills in per use — those stay as-is.

### Operational skills

| Skill | What it does |
|-------|-------------|
| `/linkedin-skills/client-build/` | Builds all 5 skills from an intake form → ready-to-zip client folder |
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

# Contributing a Skill

If you've built a Claude Code skill that works for your trade, we'd love to add it to the library.

## What makes a good skill

- Solves a specific, repeatable task (not a one-off)
- Works for any business in that trade, not just yours
- Written in plain English — no code required
- Includes at least one real example with sample input and output

## How to submit

1. Fork this repo
2. Create a new folder: `skills/your-skill-name/`
3. Add a `SKILL.md` file inside it
4. Open a pull request with a short description of what the skill does and which trade it's for

## SKILL.md format

Every skill needs this at the top:

```markdown
---
name: your-skill-name
description: Use this skill when [specific trigger]. Triggers on phrases like [examples]. Do NOT use for [what it's not for].
---
```

Then write what the skill does, what inputs it needs, and what it produces — in plain English.

Look at any of the existing 5 skills for the format to follow. `/review-responder` is the simplest example.

## Ideas for skills to build

- `/invoice-chaser` — polite payment follow-up sequence for overdue invoices
- `/complaint-handler` — structured response before it hits Google
- `/subcontractor-brief` — brief out work to a subie with your standards embedded
- `/material-order` — generate a materials list from a job description
- `/job-debrief` — end of day notes, photo checklist, job file capture
- `/warranty-claim-handler` — triage incoming warranty calls

## Questions

Open an issue or drop a comment on the LinkedIn post. Happy to help.

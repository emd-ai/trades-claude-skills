---
name: lien-waiver-generator
description: Use this skill when you need to create a lien waiver for a project payment. Triggers on phrases like "lien waiver for", "need a lien waiver", "waiver for progress payment", "final lien waiver", "GC wants a lien waiver", or "waiver before I get paid". Produces the correct waiver type based on your payment situation. Do NOT use for invoices or estimates — this is specifically for lien rights documentation.
---

# Lien Waiver Generator

**Wrong waiver = no payment or no lien rights.** This skill makes sure you pick the right type, fill it out correctly, and don't sign away your rights before the money clears.

Lien waivers are required on virtually every commercial project and many residential jobs. GCs hold payment until they receive the correct waiver. Getting this wrong delays your cash flow by days or weeks.

## The 4 types — which one do you need?

I'll ask you two questions to determine the right waiver:

**Question 1: Is this a progress payment or the final payment?**
- Progress = work is ongoing, you're billing for a portion
- Final = job is done, this is the last payment

**Question 2: Have you already received the payment?**
- No = Conditional (waiver only takes effect WHEN you get paid — safer for you)
- Yes = Unconditional (waiver takes effect immediately — only sign after money is in your bank)

| | Payment NOT yet received | Payment IS received |
|---|---|---|
| **Progress payment** | Conditional Progress | Unconditional Progress |
| **Final payment** | Conditional Final | Unconditional Final |

## What you need to tell me

- **Project name or description**
- **Project address**
- **Who hired you** (property owner or GC name)
- **Property owner name** (if different from who hired you)
- **Payment amount** (this waiver covers)
- **Through-date** (for progress waivers — the date the work is billed through)
- **Any exceptions** (disputed amounts, pending change orders, retention held)
- **Your company name**

## What I'll produce

### Conditional Waiver on Progress Payment

Use when: you're requesting a progress payment and haven't received it yet.

```
CONDITIONAL WAIVER AND RELEASE ON PROGRESS PAYMENT

Project: [Project name]
Job location: [Full address]
Owner: [Property owner name]
Name of claimant: [Your company name]
Name of customer: [GC or party who hired you]

Progress payment amount: $[Amount]
For work through: [Date]

Upon receipt of payment in the amount of $[Amount], the
claimant waives and releases any and all lien, stop-payment
notice, and payment bond rights the claimant has for labour,
services, equipment, and materials furnished through [date]
on the job described above.

EXCEPTIONS: This waiver does not cover the following
disputed claims or amounts:
[List any exceptions, or "None"]

This waiver is conditioned on receipt of payment. If the
maker of the payment fails to make the payment, this waiver
is null and void.

Claimant: ____________________________
Company: [Your company name]
Title: ________________
Date: ________________
```

### Unconditional Waiver on Progress Payment

Use when: you HAVE received the progress payment and it has cleared.

```
UNCONDITIONAL WAIVER AND RELEASE ON PROGRESS PAYMENT

Project: [Project name]
Job location: [Full address]
Owner: [Property owner name]
Name of claimant: [Your company name]

The claimant has been paid and has received progress payment
in the amount of $[Amount] for work performed through [date]
on the above-referenced project, and hereby unconditionally
waives and releases any and all lien, stop-payment notice,
and payment bond rights through that date.

EXCEPTIONS: This waiver does not cover the following
disputed claims or amounts:
[List any exceptions, or "None"]

This waiver is effective immediately upon signing.

Claimant: ____________________________
Company: [Your company name]
Title: ________________
Date: ________________
```

### Conditional Waiver on Final Payment

Use when: you're requesting your final payment (job is complete) and haven't received it yet.

```
CONDITIONAL WAIVER AND RELEASE ON FINAL PAYMENT

Project: [Project name]
Job location: [Full address]
Owner: [Property owner name]
Name of claimant: [Your company name]

Final payment amount: $[Amount]

Upon receipt of final payment in the amount of $[Amount],
the claimant waives and releases any and all lien, stop-
payment notice, and payment bond rights the claimant has
for all labour, services, equipment, and materials furnished
on the job described above.

EXCEPTIONS: This waiver does not cover the following
disputed claims or amounts:
[List any exceptions, or "None"]

This waiver is conditioned on receipt of payment. If the
maker of the payment fails to make the payment, this waiver
is null and void.

Claimant: ____________________________
Company: [Your company name]
Title: ________________
Date: ________________
```

### Unconditional Waiver on Final Payment

Use when: you HAVE received the final payment and it has cleared. **This is the most dangerous waiver to sign — make absolutely sure the money is in your bank.**

```
UNCONDITIONAL WAIVER AND RELEASE ON FINAL PAYMENT

Project: [Project name]
Job location: [Full address]
Owner: [Property owner name]
Name of claimant: [Your company name]

The claimant has been paid in full for all labour, services,
equipment, and materials furnished on the above-referenced
project, and hereby unconditionally waives and releases any
and all lien, stop-payment notice, and payment bond rights
on the project.

Final payment amount received: $[Amount]

This waiver is effective immediately upon signing.

Claimant: ____________________________
Company: [Your company name]
Title: ________________
Date: ________________
```

## Critical warnings

**NEVER sign an unconditional waiver before the money has cleared your bank.** If the cheque bounces, you've waived your lien rights AND you don't have the money. Use a conditional waiver until payment is confirmed.

**Check your state's requirements.** Some states (California, Texas, Georgia, and others) have mandatory statutory waiver forms. This skill produces standard language that works in most states, but flag any state-specific requirements you know about and I'll adjust.

**Always list exceptions.** If there are disputed amounts, pending change orders, or retention being held, list them in the exceptions section. Anything not listed is waived.

## Waiver tracker

Keep a running log for each project:

```
Project: [Name]
GC: [Name]

Date       | Waiver Type      | Amount    | Signed | Payment Confirmed
-----------|------------------|-----------|--------|------------------
[Date]     | Cond. Progress   | $[X]      | Yes    | Yes — [date]
[Date]     | Uncond. Progress | $[X]      | Yes    | Cleared [date]
[Date]     | Cond. Final      | $[X]      | Yes    | Pending
```

## Example

**You say:**
> I need a lien waiver for progress payment on the Thompson Office Renovation at 500 Main Street. Owner is Thompson Properties LLC. ABC General Contractors hired me. Payment is $8,500 for work through March 15th. I haven't been paid yet. There's a $1,200 change order still being negotiated.

**I produce:** A Conditional Waiver on Progress Payment with the $1,200 change order listed as an exception, plus a reminder not to sign the unconditional version until the $8,500 clears.

## Setup (first time only)

Tell me:
- Your company name
- Your state (for any state-specific notes)
- Your title (e.g. "Owner", "President", "Managing Member")

I'll apply these to every waiver automatically.
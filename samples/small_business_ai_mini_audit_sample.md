# Sample Deliverable: Small-Business AI Mini-Audit

This is a sample format only. A real paid audit must use the buyer's actual workflow facts and must not invent results.

## Buyer context

- Business type: small local bakery
- Workflow reviewed: Instagram DM and web form order intake
- Stated bottleneck: owner spends about 2 hours per day copying order details into a kitchen spreadsheet
- Tools already used: Instagram, Google Forms, Google Sheets

## Bottleneck summary

The workflow has three repeated manual steps:

1. Reading order messages and identifying product, pickup date, quantity, customer name, and notes.
2. Copying the details into the kitchen spreadsheet.
3. Sending a confirmation reply with pickup instructions.

## Same-day improvement plan

### Step 1: Standardize the intake prompt

Use this pinned reply or form intro:

> To place an order, please send: item, quantity, pickup date/time, name, phone/email, and any allergy notes. I’ll confirm availability before payment.

### Step 2: Use a structured extraction prompt

Paste a customer message into an AI tool with this prompt:

> Extract the order details into this exact table: Customer, Contact, Item, Quantity, Pickup Date, Pickup Time, Allergy Notes, Payment Status, Follow-Up Needed. If anything is missing, write MISSING instead of guessing.

### Step 3: Use a confirmation reply template

> Thanks, `[name]` — I have your request for `[quantity] [item]` for `[pickup date/time]`. I still need `[missing detail]` before I can confirm. Once confirmed, I’ll send payment and pickup instructions.

## Guardrails

- Do not invent missing customer information.
- Do not confirm unavailable inventory.
- Do not auto-send replies without owner review.
- Keep customer personal data inside the buyer's own approved tools.

## Handoff checklist

- [ ] Owner tests the prompt on 3 real historical messages.
- [ ] Owner updates the intake form or pinned reply.
- [ ] Owner keeps one manual review step before customer replies.
- [ ] Owner measures whether copy/paste time drops after one day.

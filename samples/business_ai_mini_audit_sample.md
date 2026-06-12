# Sample: Small-Business AI Mini-Audit Deliverable

**Service:** Small-Business AI Mini-Audit ($150)
**Client scenario:** A local bakery that takes custom cake orders via Facebook messages and phone calls. They lose track of orders, miss follow-ups, and spend too much time typing the same responses.
**This is a sample deliverable** — real projects are customized to your specific business.

---

## Workflow Reviewed: Custom Cake Order Intake (Facebook + Phone)

### Current workflow (as described by client)

1. Customer messages the bakery's Facebook page or calls.
2. Staff person responds, asks what they want (date, size, flavor, design, pickup time).
3. Conversation goes back and forth 5-10 messages to collect all details.
4. Details get written on a paper order form (sometimes lost).
5. No confirmation message sent to customer unless they ask.
6. Follow-up (pickup reminder, thank-you) happens inconsistently.

### Friction points identified

| Problem | Impact | Priority |
|---|---|---|
| Back-and-forth takes 5-10 messages per order | 15-20 min per customer, limits capacity | HIGH |
| No standard intake questions | Missed details cause rework and mistakes | HIGH |
| Paper forms get lost | Lost orders = lost revenue and unhappy customers | HIGH |
| No confirmation message | Customers uncertain if order was received | MEDIUM |
| No pickup reminder | No-shows and last-minute confusion | MEDIUM |
| No post-pickup thank-you | Missed opportunity for reviews and repeat orders | LOW |

---

## AI-Assisted Improvements

### Fix 1: Intake message template (replaces 5-10 back-and-forth messages)

Create ONE message you send immediately when someone inquires:

```
Hi [Name]! Thanks for reaching out to [Bakery Name]. We'd love to help with your cake order.

To get started, please reply with:
1. Date you need the cake
2. Number of servings
3. Flavor preference (or "surprise me!")
4. Any design ideas or theme (photos welcome!)
5. Pickup date and preferred time window
6. Your phone number (for order confirmation only — never shared)

Once we have these, we'll confirm availability and send you a total within [X hours]. A 50% deposit secures your date.

Talk soon! 🎂
```

**Time saved:** 5-10 back-and-forth messages → 1 message + 1 reply. Saves ~10-15 min per order.

### Fix 2: Digital order tracker (simple spreadsheet)

Replace paper forms with a Google Sheet (free) that tracks:

| Order # | Customer name | Phone | Date needed | Servings | Flavor | Design notes | Pickup date/time | Deposit paid | Balance due | Confirmation sent | Reminder sent | Thank-you sent |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

Share this sheet with all staff. Everyone sees all orders. Nothing gets lost.

**Template prompt to create this:** "Create a simple Google Sheets template for tracking custom cake orders with these columns: [paste columns above]. Include a second tab for completed orders."

### Fix 3: Confirmation message template

Send within 2 hours of receiving deposit:

```
Hi [Name], your [cake type] order for [date] is confirmed! 🎂

Order summary:
- [Size/servings]
- [Flavor]
- Pickup: [date] at [time]
- Balance due at pickup: $[amount]

Your order number is #[XX]. Please reference this if you need to make changes.

We'll send a pickup reminder the day before. Thank you for choosing [Bakery Name]!
```

### Fix 4: Pickup reminder template

Send 24 hours before pickup:

```
Hi [Name], just a reminder that your [cake type] pickup is tomorrow, [date], at [time].

Balance due: $[amount]
Address: [bakery address]
Order #: [XX]

Reply if you need to adjust your pickup time. Otherwise, we'll see you tomorrow! 🎂
```

### Fix 5: Post-pickup thank-you

Send 2 days after pickup:

```
Hi [Name], we hope the [cake type] was a hit! We'd love to see photos if you're willing to share — and a review on [Google/Facebook] means the world to our small business.

Thank you for choosing [Bakery Name]! 💛
```

---

## Automation Plan (no coding required)

| Step | Tool | Setup time | Ongoing time |
|---|---|---|---|
| Intake message | Saved as Facebook Page "Saved Reply" or phone notes | 5 min | 0 min |
| Order tracker | Google Sheets (shared with staff) | 15 min | 2 min per order |
| Confirmation message | Copy-paste from template, fill in details | 0 min | 2 min per order |
| Pickup reminder | Check sheet daily, send template | 0 min | 1 min per order |
| Thank-you | Check sheet weekly, send template | 0 min | 1 min per order |

Estimated total time per order: **~6 minutes** (down from ~25 minutes). At 5 orders per day, that saves ~95 minutes daily.

---

## Ready-to-use prompt templates

Use these with any AI tool:

**Prompt: Write a Facebook post about this week's cake flavors**
```
Write a friendly Facebook post for my bakery, [Bakery Name], announcing this week's featured cake flavors. Flavors: [list 2-3]. Include: a warm opening, flavor descriptions (1 sentence each), how to order (message us), and a closing with 🎂 emoji. Keep it under 100 words. Do not make up prices or offers.
```

**Prompt: Respond to a customer complaint about a late order**
```
Help me draft a kind response to a customer whose cake pickup was delayed. The situation: [briefly explain]. Rules: apologize sincerely without making excuses, offer a specific make-good ([discount on next order / partial refund / free add-on]), and invite them to reply with any concerns. Keep the tone warm and professional. Under 5 sentences.
```

---

**Disclosure:** This deliverable was created with AI assistance and human review. It is customized to the client's described business scenario. The sample business ("local bakery") is illustrative — real audits use the client's actual business details.

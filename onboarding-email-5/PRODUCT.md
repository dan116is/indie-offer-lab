# 5-Email Onboarding Sequence (For Your List)

**SKU:** `onboarding-email-5`  
**Price:** $12 USD, paid in USDC on Base  
**Format:** Five templates you load into **your** ESP  
**Audience:** US indie hackers with a paid digital product and people who opted in or bought  
**Promise:** A week of useful mail after someone pays or confirms. Not a spam cannon.

Indie Offer Lab will **not** email anyone for you. No CSV. No cold outreach.

Send only to buyers or confirmed opt-in on a form you host. CAN-SPAM: truthful subject, US postal address, working unsubscribe.

## Setup

| Field | Your value |
|---|---|
| Product / SKU |  |
| First action (&lt;20 min) |  |
| File URL |  |
| Support inbox |  |
| US postal address |  |
| ESP / from-name |  |

**Cadence:** Email 1 at purchase/confirm, then +1d, +3d, +5d, +7d. Skip 3–5 if they already did the first action.

**Footer on every mail**

```
[Your name]
[Street or PO box], [City], [ST] [ZIP]
Unsubscribe: {{unsubscribe_link}}
This is about [product], which you [bought / asked for].
```

## Email 1 — Access (immediately)

**Subject:** your [product] files + the 20-minute start

```
Hi {{first_name}},
You have [product]. Files: [URL].
Do this first: open [file], complete [first action] until you can point at [artifact].
Reply with that artifact (secrets boxed out). If the link 404s, reply with the receipt id.
[footer]
```

No second-product pitch in email 1.

## Email 2 — Stuck point (day 1)

**Subject:** if [product] feels wide, do only [narrow step]

```
Most people stall on [stuck point].
25-minute bypass: [3 concrete lines from your PRODUCT.md].
If you already passed this, ignore. If stuck on something else, reply with that sentence.
[footer]
```

## Email 3 — Labeled example (day 3)

**Subject:** what “done” looks like for [product]

Use LABELED EXAMPLES, not customers, not our revenue. No fake Stripe screenshots.

```
Example who: “Alex, US, ships a $9 markdown pack.”
Example artifact: [describe a filled template row].
Your version should use people you can already message.
[footer]
```

## Email 4 — Usage + refund (day 5)

**Subject:** still have [product] open? three checks

```
1. Files still at [URL]? Reply “resend” if not.
2. Finished [first action]? Optional two-sentence note — never required for access.
3. Corrupt or wrong SKU: [your refund line from refund-terms].
I answer email [days/hours, US timezone].
[footer]
```

Testimonials are a later optional mail (`testimonial-asks`), not this one.

## Email 5 — Optional next SKU (day 7)

**Subject:** optional: [next SKU] if [job] is still open

```
Last scheduled email about [product].
If [job] is done, unsubscribe or keep product notes. No penalty.
If you want [next SKU] it is [url] for $[price]. Same refund posture.
No countdown. No “last chance” follow-up.
[footer]
```

If you have no next SKU, **delete email 5** and say so in email 4.

## Compliance

- [ ] Only opted-in or buyers
- [ ] From-address you monitor
- [ ] US postal address on every mail
- [ ] Unsubscribe works (you clicked it)
- [ ] No purchased list, no invented results

Pay: $12 USDC on Base to `0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4`. Email `ORDER onboarding-email-5` to agent-0af2826d2bd111cc@agentmail.to with the tx hash.

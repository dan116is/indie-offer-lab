# Invoice Follow-up Emails

**SKU:** `invoice-followup-emails`  
**Price:** $12 USD, paid in USDC on Base  
**Format:** six copy-paste scripts + send-log SOP  
**Audience:** English-speaking small firms worldwide who already invoiced a client they served  
**Promise:** polite, specific follow-ups. No fake late fees. No recovery-rate claims.

Not legal advice. Not a collections playbook.

**Anti-spam:** one invoice, one thread, one human who hired you. No harvested AP lists.

## Placeholders

`{{client}}` `{{invoice_no}}` `{{amount}}` (with currency) `{{due_date}}` `{{issue_date}}` `{{work}}` `{{payment_link}}` `{{your_name}}` `{{paid_amount}}` `{{remaining}}` `{{paid_date}}` `{{receipt_no}}` `{{next_step}}`

## Calendar (from issue date; never before due date for “firm” mail)

1. Same day — invoice attached  
2. T+3 — confirm PDF arrived (skip if they confirmed or due date is weeks out)  
3. T+10 — still unpaid, due date passed  
4. T+21 — ask for a date; pause new work only if you mean it  
5. Partial payment — thanks + remaining  
6. Paid in full — receipt + next step  

If they already named a pay date, wait until it passes.

## Script 1 — same day

Subject: Invoice {{invoice_no}} for {{work}} — {{amount}} due {{due_date}}

```
Hi {{client}},

Invoice {{invoice_no}} is attached for {{work}}.
Amount: {{amount}}
Issued: {{issue_date}}
Due: {{due_date}}
Payment: {{payment_link}}

If the PDF does not match what we agreed, reply on this thread. If it looks right, no need to write back until payment is sent.

{{your_name}}
```

## Script 2 — T+3

Subject: Checking that invoice {{invoice_no}} arrived

```
Hi {{client}},

A short check that invoice {{invoice_no}} reached you. Amount {{amount}}, due {{due_date}}. PDF attached again.
If it is already in your payment run, ignore this. If the file is missing or the amount is wrong, reply and I will fix it.

{{your_name}}
```

## Script 3 — T+10 past due

Subject: Invoice {{invoice_no}} is past due ({{amount}})

```
Hi {{client}},

Invoice {{invoice_no}} for {{work}} is still open.
Amount: {{amount}}
Original due date: {{due_date}}

If this stalled on a PO, vendor record, or a missing PDF, tell me what you need. If it is in the next run, a one-line date is enough.

{{your_name}}
```

## Script 4 — T+21 firm but civil

Subject: {{invoice_no}} remains unpaid — need a payment date

```
Hi {{client}},

Invoice {{invoice_no}} for {{work}} is still unpaid ({{amount}}, due {{due_date}}).
Please send (1) a payment date you can meet, or (2) the specific blocker so I can correct paperwork.
Until this is settled I am not starting additional work beyond what we already agreed.
This email is not a legal notice and not a collections threat.

{{your_name}}
```

## Script 5 — partial

Subject: Received {{paid_amount}} on {{invoice_no}} — remaining {{remaining}}

```
Hi {{client}},

Thank you. I recorded {{paid_amount}} on {{paid_date}} against {{invoice_no}}.
Remaining: {{remaining}}
Please send the balance using {{payment_link}} with reference {{invoice_no}}.

{{your_name}}
```

## Script 6 — paid

Subject: {{invoice_no}} paid — thank you

```
Hi {{client}},

Payment for {{invoice_no}} ({{amount}}) is recorded on {{paid_date}}. Reference {{receipt_no}}.
{{next_step}}

{{your_name}}
```

## Send log

| Invoice | Client | Due | Last script | Next date | Status |
|---------|--------|-----|-------------|-----------|--------|
|  |  |  |  |  | open / paid / disputed / paused |

## Pay

Send **$12 USDC on Base** to `0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4`.  
Email `ORDER invoice-followup-emails` with `memo=invoice-followup-emails` + tx hash to `agent-0af2826d2bd111cc@agentmail.to`.

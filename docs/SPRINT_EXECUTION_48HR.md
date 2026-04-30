# 48-Hour Execution Sprint

Last updated: 2026-04-30

## Goal

By the end of 48 hours:
- Site is fully functional and credible
- 10–15 outreach messages sent
- At least 1 real conversation started

This is not a planning document. It is a checklist.

---

## Hour 0–2: Site Verification (one pass, no redesigning)

- [ ] Open site on your phone. Does it load and look right?
- [ ] Tap "Get a Free Website Review" — does it scroll to the contact section?
- [ ] Tap "Call 734-444-8558" — does it dial?
- [ ] Tap "Request a Quote" — does it open an email?
- [ ] Submit the contact form — does something happen?
- [ ] Check browser tab — does it show "Auralis Digital" not "Lovable App"?
- [ ] Open `projects/demo-index.html` — do thumbnail images load?
- [ ] Open one demo (barbershop or restaurant) — does it look credible?

If anything above fails, fix it. If everything passes, move on. Do not redesign.

---

## Hour 2–4: Formspree (lead capture backend)

- [ ] Go to formspree.io
- [ ] Create free account
- [ ] Create new form
- [ ] Copy the endpoint URL (e.g. `https://formspree.io/f/xxxxabcd`)
- [ ] Open `src/components/AuralisHomepage.tsx`
- [ ] Find line 33: `const FORMSPREE_ENDPOINT = "";`
- [ ] Paste endpoint: `const FORMSPREE_ENDPOINT = "https://formspree.io/f/xxxxabcd";`
- [ ] Commit and push to main
- [ ] Test the form by submitting it — confirm email arrives

This is the only thing still requiring account access. Everything else on the site is done.

---

## Hour 4–8: Outreach (this is the work that makes money)

Use `docs/LEADS_ACTIVE_OUTREACH.csv` — 15 businesses are already queued.

Use `docs/OUTREACH_SCRIPTS.md` — niche-specific messages are ready.

Process per business:
1. Look up the business on Google / Facebook
2. Confirm which label applies (no website vs weak presence)
3. Pick the right script from OUTREACH_SCRIPTS.md
4. Fill in business name, city, and one specific observation
5. Send via Facebook DM, Google Business, phone, or email
6. Update the CSV: set Status to "Contacted", fill in Last Contact date

Target: 10 messages sent by end of Hour 8.

---

## Hour 8–24: Follow up on replies

- Check messages every few hours
- If a reply comes in, use `docs/RESPONSE_SCRIPTS_WHEN_LEADS_REPLY_2026-04-24.md`
- If they're interested, move to `docs/CLIENT_INTAKE_QUESTIONNAIRE.md`
- If no reply yet, that is normal — follow up in 3–5 days

---

## Hour 24–48: Continue outreach + expand list

- Send 5–10 more messages to new businesses not in the current CSV
- Expand to Ypsilanti and Ann Arbor leads from `docs/EXPANSION_LEADS_VETTED_2026-04-24.md`
- Log every business contacted in the CSV
- Keep messages short and niche-specific

---

## What "First Conversation" Looks Like

Any reply counts. Even:
- "Not interested right now"
- "We already have someone"
- "Can you send more info?"

A reply is signal. Learn from it. Ask a follow-up question.

If they say they're interested: do not pitch immediately. Ask:
> "What does your current online presence look like? Are you looking for a refresh or starting fresh?"

Then use the intake questionnaire.

---

## What Success Looks Like After 48 Hours

| Metric | Target |
|---|---|
| Site passes phone check | ✓ |
| Formspree active | ✓ |
| Messages sent | 10–15 |
| Replies received | 1–3 |
| Real conversation started | 1 |

---

## What to Ignore for the Next 48 Hours

- Do not redesign the homepage
- Do not add new features
- Do not research new tools
- Do not rewrite the docs
- Do not wait until the site is "perfect"

The site is ready enough. The only thing that makes money is the conversation.

---

## After the Sprint

If a lead is interested → `docs/CLIENT_INTAKE_QUESTIONNAIRE.md`
If they say yes → `docs/QUOTE_AND_SCOPE_TEMPLATE.md`
If they sign → `docs/FIRST_CLIENT_DELIVERY_CHECKLIST.md`
After delivery → `docs/CLIENT_PROOF_WORKFLOW.md`

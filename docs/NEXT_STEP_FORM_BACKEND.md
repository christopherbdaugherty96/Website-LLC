# NEXT STEP: Form Backend (Formspree)

Status: immediate next action

## Why this matters

The current site is live and functional, but lead capture still relies on mailto links. This is unreliable and reduces conversions.

A real form backend turns the website into a working lead system.

---

## Goal

Replace mailto-based contact flow with a real form submission system using Formspree.

---

## What Formspree Does

User fills out form → clicks submit → Formspree processes submission → sends to Auralis email.

No backend or server setup required.

---

## Steps

1. Go to https://formspree.io
2. Create a free account
3. Create a new form
4. Copy the endpoint URL (example: https://formspree.io/f/xxxxabcd)

---

## Code Update

Open:

src/components/AuralisHomepage.tsx

Find:

const FORMSPREE_ENDPOINT = "";

Replace with:

const FORMSPREE_ENDPOINT = "https://formspree.io/f/xxxxabcd";

---

## Deploy

Commit and push to main.

GitHub Actions will rebuild and deploy automatically.

---

## Test

- Submit form on live site
- Confirm email is received
- Confirm no errors on submission

---

## Success Criteria

- Form submits without opening email app
- Submission arrives in inbox
- Contact flow feels immediate and reliable

---

## Internal Note

This is the final step required to turn the site from a static presentation into an actual lead-generation tool.

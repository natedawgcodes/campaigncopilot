---
name: website-copy-builder
description: >-
  Generate ready-to-publish copy for a political campaign website, page by page.
  Use when a campaign or digital staffer needs website copy or is building out a
  campaign site. Triggers on requests like "write our campaign website copy",
  "I need homepage and about page copy", "draft the issues and volunteer pages",
  "give me the donate page with form fields", or "write SEO titles and meta
  descriptions for the site". Produces, per page, a headline, subhead, body, a
  call to action, suggested form fields, an SEO title, and a meta description.
  Covers home, about, issues, volunteer, donate, endorsements, event, and contact
  pages. Reads references/intake.md first.
---

# Website Copy Builder

This skill writes a campaign website one page at a time, with copy that is
consistent across pages and structured so a developer or site builder can drop it
straight in, including the form fields and the search metadata.

## Step 1: Read the intake

Read `references/intake.md` to confirm the core message, the top issues, the bio
basics, the endorsements and events, the donation and contact details, the tone
and brand words, and the SEO keywords (candidate name, office, location).

Collect what you can from the user's request and ask for the essentials that are
missing: candidate and office, the core message, the top issues, and the donation
link. Confirm which pages to build; default to the full set below if the user does
not specify.

## Step 2: Build each page using this exact structure

For every requested page, produce all of these fields:

```
## [Page name]

- Headline: the main promise or invitation on the page.
- Subhead: one line that supports the headline.
- Body: the page copy, in short web-friendly paragraphs.
- Call to action: the button or link text and where it goes.
- Form fields: the fields this page's form should collect (or "none" if the page
  has no form).
- SEO title: about 60 characters, including the candidate name and office.
- Meta description: about 150 to 160 characters that earns the click.
```

### Pages to cover

- **Home:** the core message, the top issues at a glance, and the primary call to
  action. Form fields: email and zip capture.
- **About:** the candidate's story and why they are running. Form fields: none or
  a sign-up prompt.
- **Issues:** the top issues, each a short section. Form fields: none.
- **Volunteer:** the ask and the ways to help. Form fields: name, email, phone,
  zip, interests.
- **Donate:** the reason to give and the ask ladder. Form fields: defer to the
  donation platform; include the call to action and disclaimer placeholder.
- **Endorsements:** who backs the candidate and a representative quote. Form
  fields: none.
- **Event:** an event page with the details and an RSVP. Form fields: name, email,
  number attending.
- **Contact:** how to reach the campaign and the press. Form fields: name, email,
  message.

Write the real copy for each page. Keep the headline voice and the core promise
consistent across all pages.

## Guidance

- **One core message, repeated.** Every page should feel like the same campaign.
  Reuse key phrases from the core message on purpose.
- **Web copy is short.** Lead with the headline and the call to action. Bodies are
  scannable paragraphs and bullets, not essays.
- **Every page has one primary action.** Decide it (sign up, volunteer, donate,
  RSVP) and make it the clearest thing on the page.
- **Write SEO for humans first.** The SEO title and meta description should read
  naturally while including the candidate name, office, and location.
- **Disclaimer on the donate page.** Include the paid-for placeholder for the user
  to confirm; this is awareness, not legal advice.

## References

- `references/intake.md`: fields to collect before writing the pages.

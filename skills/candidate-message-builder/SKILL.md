---
name: candidate-message-builder
description: >-
  Turn a candidate's background, issues, and reason for running into a
  disciplined, reusable message set for a political campaign. Use when a
  candidate or consultant needs core messaging, a stump pitch, bios, or
  ready-to-use copy across formats. Triggers on requests like "build our core
  message", "write the candidate's stump speech pitch", "I need a short and long
  bio", "draft our website hero and palm card", or "give me the message in SMS
  and social versions". Produces a core message, stump pitch, short and long bio,
  website hero, palm card, volunteer pitch, and SMS and social versions, all
  consistent with each other. Reads references/intake.md first.
---

# Candidate Message Builder

This skill builds one consistent message and then expresses it across every
format a campaign needs. The point is discipline: the core message comes first,
and every other piece is the same message sized for a different surface, not a new
idea each time.

## Before you start: load the campaign profile

Check the user's working directory for a `campaigns/` folder before asking for any
shared context.

- If exactly one profile exists (for example `campaigns/jane-miller.md`), load it
  and treat it as the source of shared campaign context.
- If several profiles exist, ask which campaign this is for, then load that one.
- If none exists, let the user know they can run the `campaign-setup` skill first to
  capture shared context once, so they do not re-enter it for every skill. Offer to
  proceed now by asking for the shared fields inline.

Reuse these shared fields from the profile without re-asking: candidate name, office,
district or jurisdiction, party, opponent(s), top issues, default tone, and key
dates. The profile's notes section may also carry do-not-say language, a slogan, or
endorsements, so check there too. Then continue with the intake step below and ask
only for the per-task fields the profile does not already provide.

## Step 1: Read the intake

Read `references/intake.md` to confirm the candidate's biography, the top issues,
why they are running, the values and tone, and any contrast with the opponent.

Collect what you can from the user's request and ask for the essentials that are
missing: candidate and office, top three issues, the biographical facts, and why
the candidate is running. If you must use a placeholder (for example, a specific
accomplishment), label it so it is easy to fill in.

## Step 2: Write the core message first

Before any other piece, write the core message: two or three sentences that say
who the candidate is, what they will fight for, and why it matters now. Everything
else derives from this. Get the user's read on it if possible, because a weak core
message makes every downstream piece weak.

## Step 3: Build the full set using this exact structure

```
# Message set: [candidate], [office]

## Core message
Two or three sentences. The foundation for everything below.

## Stump pitch
60 to 90 seconds of spoken copy: open, the why, the top issues, the ask.

## Short bio
About 50 words. For introductions and program listings.

## Long bio
About 150 to 250 words. For the website about page and press.

## Website hero
A headline and one or two supporting lines for the top of the homepage.

## Palm card
Front and back copy: name, office, a tagline, three to five issue bullets, and
a call to action. Keep it scannable.

## Volunteer pitch
A short, warm ask that tells a supporter why to get involved and what to do
first.

## SMS version
One short message in the candidate's voice that identifies the campaign.

## Social version
A post-length version with a hook, the core idea, and a call to action.
```

Write the real copy for each. Keep the voice and the central promise identical
across all of them; only the length and format change.

## Guidance

- **Consistency is the product.** A voter who sees the palm card, the website, and
  a text should hear the same campaign. Reuse key phrases on purpose.
- **Concrete beats abstract.** Name the issue and what the candidate will do, not
  vague values alone.
- **Lead with the voter, not the resume.** The bio earns trust, but the message is
  about the voter's life. Even the long bio should connect to why it matters to
  them.
- **Match the tone from intake.** Professional, populist, or neighborly should
  read consistently across every piece.

## References

- `references/intake.md`: fields to collect before building the message set.

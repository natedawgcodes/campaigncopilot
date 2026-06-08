---
name: fundraising-generator
description: >-
  Build a complete multi-touch fundraising ask for a political campaign, not a
  single email. Use when a campaign, finance staffer, or consultant needs a
  donor appeal across email, SMS, and a donation page. Triggers on requests like
  "write a fundraising email", "build an end-of-quarter ask", "we need a donor
  appeal with subject lines and a resend", "draft a fundraising text", or "set up
  a 3-touch fundraising sequence". Produces five subject lines, preview text, a
  main email, a shorter resend, an SMS version, a donation-page call to action,
  and a 3-touch follow-up sequence. Includes disclaimer and opt-in placeholders
  as compliance awareness, not legal advice. Reads references/intake.md first.
---

# Fundraising Generator

This skill builds a full fundraising push, because money rarely comes from one
send. It produces a coordinated set of asks across channels and a follow-up
sequence, all built around one reason to give now.

## Step 1: Read the intake

Read `references/intake.md` to confirm the candidate, the ask (deadline and
goal), the reason for urgency, the audience, the suggested amounts, the sender,
and the compliance inputs (required disclaimer text, SMS opt-in source, and
donation link).

Collect what you can from the user's request and ask for the essentials that are
missing: candidate and office, the reason for the ask, the deadline or goal, the
audience, and the donation link. If a required disclaimer is unknown, use a clear
placeholder such as `[PAID FOR BY ...]` and flag it.

## Step 2: Find the one reason to give now

Every effective ask has a specific, honest reason to give today: a deadline, a
match, a news moment, a goal to hit. Establish that first. A general "please
donate" underperforms a concrete "we are 200 donors short before Friday's
deadline." Do not fabricate urgency; use the real reason from the intake.

## Step 3: Build the full push using this exact structure

```
# Fundraising push: [candidate], [purpose]

## Subject lines (5)
Five options in different styles (urgent, personal, curiosity, news hook,
straightforward). Note which audience each suits.

## Preview text
The inbox preview line that pairs with the subject.

## Main email
The full appeal: hook, the reason to give now, what the money does, the ask with
suggested amounts, and a clear button line. Includes the disclaimer placeholder.

## Resend
A shorter version for non-openers, with a different subject. Same ask, less
build-up.

## SMS version
One short message: who it is from, the reason, the ask, the link, and an opt-out
(for example, "Reply STOP to opt out").

## Donation-page call to action
The headline and short copy on the contribution page so the message carries
through to the point of giving. Include the ask ladder.

## 3-touch follow-up sequence
Three sends across the push window (for example, kickoff, midpoint reminder, final
deadline), each with a subject and short body and an escalating sense of the
deadline.
```

Write the real copy. Keep the reason to give consistent across every touch.

## Guidance

- **One clear ask, one clear reason.** Mixed asks lower response. Pick the goal
  and the deadline and hold them across the push.
- **Suggested amounts help.** An ask ladder (for example, a few specific dollar
  amounts) outperforms an open field. Use the amounts from the intake.
- **Match the sender's voice.** A note from the candidate, the manager, or a
  family member reads differently. Write to the named sender.
- **Make giving frictionless.** Put the link early and repeat it. The donation
  page copy should match the email so the donor knows they are in the right place.

## Compliance awareness (not legal advice)

Treat these as operational reminders, not legal advice:

- **Disclaimer placeholders.** Include the required paid-for or authorization
  disclaimer as a clear placeholder (for example, `[PAID FOR BY THE COMMITTEE TO
  ELECT ...]`) wherever it belongs. The user supplies and confirms the exact
  text.
- **SMS opt-in awareness.** Fundraising texts should go only to recipients with a
  valid opt-in, and every message offers a way to opt out.
- **Contribution rules.** Suggested amounts and solicitations are subject to
  contribution limits and source restrictions that vary by jurisdiction and
  office.

The user is responsible for confirming the legal requirements for their own
jurisdiction, including disclaimers, contribution limits, and texting rules. This
skill does not provide legal advice.

## References

- `references/intake.md`: fields to collect before building the push.

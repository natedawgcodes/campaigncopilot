---
name: press-release-writer
description: >-
  Write a complete, ready-to-send press release for a political campaign, plus
  the pitch and social copy that go with it. Use when a campaign or comms staffer
  needs to put out news: an announcement, endorsement, policy rollout, event
  advisory, response to an attack, or a crisis holding statement. Triggers on
  requests like "write a press release announcing our campaign", "draft an
  endorsement release", "we need a statement responding to the attack", "put out
  an event advisory", or "I need a holding statement". Produces a headline,
  subhead, dateline, body, candidate quote, manager quote, boilerplate, a
  reporter pitch email, and a social version. Reads references/intake.md first.
---

# Press Release Writer

This skill writes a press release a campaign can send as-is, in the right shape
for the type of news, with the pitch email and social copy that turn a release
into coverage.

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

Read `references/intake.md` to confirm the release type, the news and its key
facts, the spokespeople and quotes, the press contact, the dateline, and the
boilerplate.

Collect what you can from the user's request and ask for the essentials that are
missing: the release type, the core news (who, what, when, where, why), and the
press contact. Use clear placeholders for anything unknown (for example,
`[PRESS CONTACT NAME, PHONE, EMAIL]`) and flag them.

## Step 2: Match the type

The type sets the shape. Confirm which one before writing:

- **Announcement:** lead with the news and why it matters now.
- **Endorsement:** lead with the endorser and a quote on why; show what it
  signals.
- **Policy:** lead with the problem and the candidate's plan; include a proof
  point or two.
- **Event advisory:** who, what, when, where, and visuals, in a scannable
  format, with RSVP details. Advisories are shorter than full releases.
- **Response to attack:** brief, factual, on offense where possible; do not
  repeat the attack's framing.
- **Crisis holding statement:** short, calm, says what is known and what comes
  next; commits to nothing unconfirmed.

## Step 3: Build the release using this exact structure

```
FOR IMMEDIATE RELEASE (or embargo line)
[Date]
Contact: [name, phone, email]

# Headline
A subhead that adds the second most important fact.

[CITY, STATE] - [Date] - Opening paragraph with the core news (who, what, when,
where, why).

Body paragraphs: context, detail, and proof points in descending order of
importance.

"Candidate quote that sounds like a person and advances the message,"
said [Candidate], [title or office sought].

"Manager or surrogate quote that adds a second voice or frames the stakes,"
said [Name], [title].

Closing paragraph: what happens next or the call to action.

### Boilerplate
A short standing paragraph about the candidate and campaign.

###
(end mark)
```

Then add:

```
## Reporter pitch email
A short subject line and a three to five sentence email to a reporter: why this is
news for their readers, the one line that matters, and an offer (interview,
details). Less formal than the release.

## Social version
A post-length version of the news with a hook and, where relevant, a link.
```

For an event advisory, use the who, what, when, where, visuals, RSVP format
instead of the full release body.

## Guidance

- **Most important fact first.** Reporters read the top and stop. Put the news in
  the headline and the first sentence.
- **Quotes should sound human.** A quote that reads like a press release is dead
  weight. Make it sound like the person said it.
- **Response releases stay disciplined.** Be brief and factual, lead with the
  truth, and do not amplify the attack by repeating it.
- **Holding statements promise process, not conclusions.** Say what is known,
  show seriousness, and commit only to following up.

## References

- `references/intake.md`: fields to collect before writing the release.

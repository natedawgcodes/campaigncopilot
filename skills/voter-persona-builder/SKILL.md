---
name: voter-persona-builder
description: >-
  Define and profile target voter segments for a political campaign and match a
  tailored message to each. Use when a campaign staffer, organizer, or consultant
  needs voter personas, audience segmentation, or message-to-segment matching.
  Triggers on requests like "build voter personas for our race", "who are our
  target segments and what do we say to each", "segment our universe and match
  messaging", or "persona for suburban swing voters". Produces, per segment:
  core concern, motivating issue, emotional frame, best messenger, best channel,
  do-not-say language, and a sample line for door, SMS, and mail. Reads
  references/intake.md and references/segment-library.md first.
---

# Voter Persona Builder

This skill turns what a campaign knows about its electorate into a small set of
working voter personas, each with a message matched to it. A useful persona is
grounded in the campaign's real universe, not a stereotype, and it ends in
language a volunteer or writer can actually use across door, SMS, and mail.

## Step 1: Read the intake and the segment library

Read `references/intake.md` to see what the persona set depends on (the race, the
voter universe and data the campaign actually has, the top issues, and any
do-not-say language from the candidate). Then read `references/segment-library.md`
for common segments to use as starting hypotheses.

Collect what you can from the user's request. Ask for the essentials that are
missing: the office, the jurisdiction, the top issues, and what the campaign
knows about its voters (turnout history, party registration, geography, or just
what organizers hear at the doors). If the user wants a draft now, proceed and
mark assumptions clearly so they are easy to correct.

## Step 2: Choose the segments for this race

Pick three to six segments that matter for this specific race. Start from
`segment-library.md`, but adapt every segment to the local universe. A segment is
worth a persona only if the campaign would actually talk to it differently. If
two draft segments would hear the same message through the same channel, merge
them.

Name each segment in plain campaign language (for example, "soft-support parents
in the north precincts," not "Segment C").

## Step 3: Build each persona using this exact structure

For every segment, produce all of these fields, in this order:

```
## [Segment name]

- Core concern: the worry that actually drives this voter's decision.
- Motivating issue: the campaign issue that speaks to that concern.
- Emotional frame: the feeling the message should evoke (for example,
  reassurance, pride, urgency, belonging).
- Best messenger: who this voter trusts to carry the message (the candidate, a
  neighbor, a local leader, a trusted institution).
- Best channel: where this voter is reachable and receptive (door, phone, SMS,
  mail, digital).
- Do-not-say: words, claims, or framings that backfire with this segment, plus
  any candidate do-not-say from the intake.
- Sample lines:
  - Door: one or two sentences a canvasser can say.
  - SMS: one short message, identifies the campaign, fits about one segment.
  - Mail: one headline or pull quote for a mail piece.
```

Write the real copy in each field. The sample lines should sound like the
emotional frame and avoid the do-not-say list.

## Field guidance

- **Core concern vs motivating issue.** The concern is the human worry (can I
  afford to stay in this town). The issue is the campaign's answer to it
  (property tax relief). Lead persuasion with the concern, then the issue.
- **Emotional frame.** Match it to the concern. Anxious voters need reassurance
  before a call to action; proud voters respond to belonging and momentum.
- **Best messenger.** Voters discount messages from sources they distrust. Naming
  the right messenger is often more decisive than the words.
- **Do-not-say.** This is where personas earn their keep. Note the framings that
  read as condescending, off-key, or out of touch for this segment.

## Grounding and ethics

Personas are hypotheses to validate against the campaign's own data and what
organizers hear in the field, not fixed truths about groups of people. Keep them
respectful: describe what a voter cares about and how to reach them, never in
terms that demean or reduce them to a stereotype. When the data is thin, say so
and frame the persona as a starting point to test, not a conclusion.

## References

- `references/intake.md`: fields to collect before building personas.
- `references/segment-library.md`: common segments as starting points, not
  prescriptions.

---
name: field-script-builder
description: >-
  Generate structured, ready-to-run voter-contact scripts for political campaign
  field programs. Use when a campaign staffer, organizer, or consultant needs a
  door canvass, phone bank, or SMS script for voter ID, persuasion, GOTV,
  volunteer recruitment, or ballot chase. Triggers on requests like "write a
  canvass script", "phone bank script for our turnout push", "GOTV text for early
  voters", "persuasion script on housing", "volunteer recruitment call", or
  "ballot chase script for mail voters". Produces a script with goal, target
  audience, opening, question flow, objection handling, the voter-file data to
  collect, a closing ask, and follow-up. Reads references/intake.md to gather
  campaign details first.
---

# Field Script Builder

This skill produces a structured voter-contact script for a campaign field
program. A good field script is short, sounds like a real person, moves toward
one clear ask, and captures clean data back to the voter file. That is the bar
to hit.

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

## Step 1: Read the intake first

Before writing anything, read `references/intake.md`. It lists the fields a
script depends on (candidate, office, contact method, purpose, top issues, voter
segment, tone, local specifics, and compliance notes).

Collect what you can from the user's request. For anything essential that is
missing, ask for it: candidate and office, contact method, purpose, the top
issues, and the voter segment. Do not stall the user, though. If they want a
draft now, write it with clearly labeled placeholders (for example,
`[CANDIDATE NAME]`, `[ELECTION DATE]`) and list your assumptions at the top so
they are easy to fill in or correct.

## Step 2: Lock the method and purpose

Two choices shape the whole script. Confirm both before writing.

- **Contact method:** door canvass, phone bank, or SMS.
- **Purpose:** voter ID, persuasion, GOTV, volunteer recruitment, or ballot chase.

The method sets length, tone, and format. The purpose sets the question flow and
the closing ask. Method guidance is below under "Method specifics" and purpose
guidance under "Purpose specifics."

## Step 3: Build the script using this exact structure

Every script uses these sections, in this order:

```
# [Purpose] script: [Method] for [Candidate], [Office]

## Goal
One line. The single outcome a volunteer should drive toward.

## Target audience
The voter segment this script is for, and what we assume about them.

## Opening
Confirm you are speaking with the right voter, identify yourself, and identify
the campaign. Keep it to a few seconds.

## Body / question flow
The ordered questions or talking points for this purpose. Mark where the
volunteer pauses to listen.

## Objection handling
The two or three objections most likely here, each with an acknowledge,
redirect, reask bridge. Pull these from references/objection-handling.md.

## Data to collect
The fields to record back to the voter file or CRM (see "Data to collect" below).

## Closing ask
The one concrete commitment to request, matched to the purpose.

## Follow-up / next action
What happens after the contact: tag in the CRM, schedule a callback, or confirm
by text.
```

Write the actual script copy inside each section, not a description of it. A
volunteer should be able to read it aloud as-is.

## Method specifics

**Door canvass.** Warm and conversational. The voter can see you, so lead with a
friendly greeting and read the room. Keep the whole interaction to a couple of
minutes. Write stage directions in brackets, for example `[hand them lit]` or
`[if not home, leave door hanger and mark on the app]`.

**Phone bank.** No visual cues, so the opening has to confirm identity and
campaign fast and give the voter a reason to stay on. Keep questions short and
front-load the most important one in case they hang up. Include a voicemail line.
Note do-not-call awareness in the compliance section.

**SMS.** Short and plain. Identify the campaign in the first message, since the
voter may not have the number saved. Keep each message to roughly one segment
(about 160 characters) and say so where a message runs long. Include a clear
opt-out (for example, "Reply STOP to opt out"). Write it as a short back-and-forth
with branches for likely replies (yes, no, question, STOP). Note TCPA and opt-in
awareness in the compliance section.

## Purpose specifics

**Voter ID.** The job is to learn where the voter stands and record it cleanly.
Ask the support question plainly and capture a support score from 1 to 5. Ask
which issue matters most to them. Keep persuasion light; the goal is an honest
read, not a conversion.

**Persuasion.** Lead with two or three short persuasion points keyed to the
campaign's top three issues from the intake, in the candidate's framing. Make one
point, listen, and respond to what the voter actually says rather than reciting
all three. A contrast with the opponent is optional. If you include one, follow the
opponent-contrast rule below: any factual claim about the opponent must carry a
verification flag and is never stated as settled. Close by re-checking the support
score to measure movement.

**GOTV.** Assume the voter already supports the candidate; do not re-litigate.
Run a plan-to-vote sequence: ask when they plan to vote, how (in person on
election day, early in person, or by mail), and where their polling place or drop
location is. Lock a specific day and time, and offer a reminder. Use the election
date and early-vote dates from the intake.

**Volunteer recruitment.** Make a direct ask to help, then offer a short menu of
roles (knock doors, make calls, send texts, host or staff an event). Lower the
barrier with a specific first shift and time rather than an open-ended "let us
know." Capture interest and the best way to follow up. Pull recruitment
objections from references/objection-handling.md.

**Ballot chase.** For voters who requested or were mailed a ballot. Confirm they
received it, remind them of the return deadline, and offer the return options
(mail, drop box, or in person). If your jurisdiction has a signature cure
process, note it as a reminder. Record ballot status so chased voters drop off
the list once they return it.

## Opponent contrast: flag every factual claim for verification

A persuasion script may draw a contrast with the opponent, but a canvasser must
never be handed an unverified factual claim to say as fact. This is a standing rule,
not a stylistic choice, and it applies anywhere a contrast appears, including the
persuasion body and the objection-handling bridges.

Whenever a contrast line asserts a specific factual claim about the opponent (a vote,
a date, a position, a number, or any point of record), do both of these in the script
itself:

- Attach a visible verification flag right where the claim appears, as a bracketed
  stage direction, for example `[Verify against the public record before using this
  line.]`. Do not bury it in a footnote; it sits next to the words the canvasser
  reads.
- Phrase the line so it is easy to drop or correct if the record does not back it.
  Never present the claim as settled.

If a claim cannot be tied to the public record, do not put it in the canvasser's
mouth at all. A general, checkable contrast (for example, "Jane has a plan on the
reassessment, and the incumbent has had two terms") is safer than a specific
assertion the campaign has not confirmed. The campaign owns verifying the record; the
script's job is to make sure no unverified claim goes out as fact.

## Data to collect

This is the line that ties a script to the voter file or CRM. Every script
records, where relevant to the purpose:

- **Support score, 1 to 5** (5 is strong support, 1 is strong opposition).
- **Issue priority:** the issue the voter named as most important.
- **Vote method:** in person on election day, early in person, or by mail.
- **Volunteer interest:** yes or no, and preferred role if yes.
- **Contact info updates:** corrected phone, email, or address.

Write these as quick fields the volunteer can mark, not as extra questions to
interrogate the voter with. Collect what fits the conversation.

## Objection handling

Read `references/objection-handling.md` and pull the two or three objections most
likely for this method and purpose. Use the acknowledge, redirect, reask bridge:
acknowledge what the voter said so they feel heard, redirect to the campaign's
point, then reask the original question. Stay warm and never argue.

Disengaging is part of the script, not a failure. On hostility or any
do-not-contact request, stop the bridge: thank them, end politely, and mark the
record so they are not contacted again. The objection file spells out exactly
when to disengage.

## Compliance awareness (not legal advice)

Treat all compliance notes as operational reminders and awareness placeholders,
not legal advice. Build them into the script as short standing reminders:

- **SMS scripts:** note TCPA and opt-in awareness. The voter should be on a list
  with a valid opt-in source, and every message gives a way to opt out.
- **Phone scripts:** note do-not-call awareness. Respect do-not-call status from
  the voter file and honor any request to stop.
- **All scripts:** identify the campaign clearly in the opening.

State plainly in the script that the user is responsible for confirming the legal
requirements for their own jurisdiction (TCPA, state telemarketing and texting
rules, do-not-call lists, and any disclaimer or paid-for language). This skill
does not provide legal advice.

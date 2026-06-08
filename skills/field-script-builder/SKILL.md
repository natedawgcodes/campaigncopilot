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
all three. A contrast with the opponent is optional and should stay factual. Close
by re-checking the support score to measure movement.

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

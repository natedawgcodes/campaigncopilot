---
name: campaign-setup
description: >-
  Capture a campaign's shared context once and store it in a portable profile
  file that the other Campaign Copilot skills read first, so staff stop
  re-entering the same details for every task. Use at the start of working with
  the pack, or when adding or updating a campaign. Triggers on requests like "set
  up my campaign", "create a campaign profile", "get started", "add a new
  campaign", "update our candidate profile", or "save our race details". Runs a
  short conversational intake (candidate, office, district, party, opponent, top
  issues, tone, key dates, notes), then writes campaigns/<name>.md and confirms
  the filename. Reads references/intake.md and references/profile-template.md
  first.
---

# Campaign Setup

This skill captures a campaign's shared context one time and saves it to a
portable profile file the rest of the pack reads first. Instead of re-answering
the same questions (candidate, office, district, opponent, issues, tone) for every
script, release, or persona, the user fills this in once and every other skill
pulls from it. Consultants running several races keep one profile per campaign.

## Step 1: Read the intake and the template

Read `references/intake.md` for the fields to gather and the order to ask them in.
Read `references/profile-template.md` for the exact file format to write.

## Step 2: Check for existing profiles

Look for a `campaigns/` folder in the user's working directory.

- If it does not exist, you will create it when you write the first profile.
- If it exists and already holds one or more profiles, list them and ask whether
  to create a new campaign or update an existing one. To update, load that file
  first and confirm changes against what is already there rather than overwriting
  it blindly.

## Step 3: Run the intake as a conversation

Ask one topic at a time, the way a staffer would actually talk it through, not as a
wall of blank fields. Confirm anything the user has already told you instead of
re-asking, group related questions, and keep it moving. Work through the topics in
this order: candidate and office, district, party (optional), opponent(s), top
three issues, default tone, key dates, and notes.

Do not stall the user. If they want to skip a field, leave it clearly blank in the
file (for example, `Opponent(s): [TBD]`) so it is easy to fill in later, and move
on.

## Step 4: Write the profile and confirm it

Derive the filename from the candidate name: lowercase, hyphenated. "Jane Miller"
becomes `campaigns/jane-miller.md`. Write the file using
`references/profile-template.md`, keeping the field labels exact so the other
skills can read them and the layout readable so the user can hand-edit it.

Then confirm the exact path you wrote back to the user, and let them know the other
skills will read it automatically from now on. If you updated an existing profile,
summarize what changed.

## Keep the profile private (awareness, not legal advice)

The `campaigns/` folder holds campaign-internal information: opponent research,
tone and strategy decisions, and race notes. It should not be committed to a public
repository. The pack ships a `.gitignore` that excludes `campaigns/` by default,
but say this plainly so the user knows the profile is internal and stays on their
own machine or in a private location.

## References

- `references/intake.md`: the fields to gather, grouped and in ask order.
- `references/profile-template.md`: the exact markdown format for
  `campaigns/<name>.md`.

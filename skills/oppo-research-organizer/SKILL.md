---
name: oppo-research-organizer
description: >-
  Organize public information that the user provides into a structured opponent
  vulnerability memo for a political campaign. Use when a staffer or consultant
  has gathered public-record material on an opponent and needs it structured into
  a usable memo. Triggers on requests like "organize this oppo into a memo",
  "structure my research on the opponent", "build a vulnerability memo from these
  sources", or "turn these public records into a contrast brief". Produces an
  executive summary, top vulnerabilities, a source-logged timeline, a public
  quote bank, contrast opportunities, a risk level, and follow-up research
  needed. This skill organizes and structures material the user supplies. It does
  not search for, infer, or fabricate information about anyone. Reads
  references/intake.md and references/source-logging.md first.
---

# Oppo Research Organizer

This skill structures opposition research that the user has already gathered. It
takes public-record material the user provides and organizes it into a clear,
sourced vulnerability memo a campaign can act on.

## What this skill does and does not do

Read this before anything else, and state it back to the user in the memo.

- It organizes and structures information the user provides.
- It does not search for, dig up, guess at, or invent information about an
  opponent or anyone else. If the user has not provided a fact, it does not
  appear in the memo.
- Every claim in the memo traces to a source the user supplied and logged. A
  point with no source does not belong in the memo; it goes under follow-up
  research needed instead.
- It works only with public-record and on-the-record material. See
  `references/source-logging.md` for what qualifies. Private, rumored, or
  improperly obtained material is excluded.

If the user asks the skill to find dirt, fabricate a claim, or include something
unsourced, decline and explain that this skill only organizes verifiable
public material the user provides.

## Step 1: Read the intake and the source-logging guide

Read `references/intake.md` to confirm the subject, the race context, the
campaign's own positions (needed for contrast), and the materials the user is
providing. Read `references/source-logging.md` for how to log and rate each
source and what counts as public record.

If the user has provided raw material, work from it. If key context is missing,
ask for it. Do not fill gaps with assumptions about the opponent.

## Step 2: Log and rate every source first

Before writing the memo, build the source log using `source-logging.md`. Each
item gets a citation, a date, a type, where it can be found, and a reliability
rating. The memo is only as strong as its weakest cited source, so this step
gates everything after it.

## Step 3: Build the memo using this exact structure

```
# Opponent vulnerability memo: [opponent name], [office]

## Scope note
One line stating this memo organizes public, user-provided material only, and
includes no unsourced claims.

## Executive summary
Three to five sentences: the strongest, best-sourced findings and the overall
picture.

## Top vulnerabilities
The most significant findings, ranked. For each: the claim, the source (from the
log), the date, and why it matters to voters. Drop any item that lacks a source.

## Timeline
Source-logged chronology of relevant public actions and statements. Each entry
carries its date and source.

## Public quote bank
Direct, on-the-record quotes from the opponent, each with source and date and
enough context to be fair.

## Contrast opportunities
Where the opponent's public record differs from the campaign's positions. State
both sides factually.

## Risk level
For each major finding, rate how usable it is (see below) and flag anything that
could backfire or is not solid enough to use yet.

## Follow-up research needed
Open questions and unsourced leads to verify through public records before use.
This is where anything unverified lives.
```

## Rating usability and risk

For each major finding, give a plain rating:

- **Solid:** well sourced from strong public record, fair in context, ready to
  use.
- **Usable with care:** real but needs framing, more context, or a second source.
- **Not yet usable:** thin, single weak source, or easy to rebut. Move it to
  follow-up research needed rather than top vulnerabilities.

Flag findings that could backfire (stale, out of context, or likely to generate
sympathy) so the campaign decides with eyes open.

## Compliance and ethics

Treat this as operational guidance, not legal advice. Use only public-record and
on-the-record material the user provides. Keep the focus on the opponent's public
actions, votes, statements, and filings, not private life. The user is
responsible for confirming the accuracy of the underlying material and that its
gathering and use comply with the law and platform rules in their jurisdiction.

## References

- `references/intake.md`: fields to collect before organizing.
- `references/source-logging.md`: how to log and rate sources, and what counts as
  public record.

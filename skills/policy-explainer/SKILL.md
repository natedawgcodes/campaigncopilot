---
name: policy-explainer
description: >-
  Turn a candidate's policy position into clear, voter-ready language for a
  political campaign. Use when a campaign or policy staffer needs to explain a
  position so voters understand it, care about it, and can defend it. Triggers on
  requests like "explain our housing plan in plain English", "make this policy
  voter-ready", "why should voters care about this position", "give me the
  30-second version and the door version", or "what are the objections and
  rebuttals". Produces a plain-English explanation, why voters should care, local
  impact, common objections, simple rebuttals, a 30-second answer, a website
  section, and a door version. Frame and tone come from the intake, not from
  assumption. Reads references/intake.md first.
---

# Policy Explainer

This skill translates a policy position into language voters actually use. It
takes the candidate's real position and the frame the campaign chose, and
produces explanations sized for the website, the doors, and a quick answer, plus
the objections and rebuttals to hold the line.

## Step 1: Read the intake

Read `references/intake.md` to confirm the position itself, the goal of the
policy, the supporting facts, the local impact, the frame and values to use, the
audience, and the opponent's contrasting position if any.

Collect what you can from the user's request and ask for the essentials that are
missing: the actual position, what it is meant to achieve, and the frame to use.
Do not invent the candidate's position or its details; ask.

## Step 2: Use the provided frame, do not assume one

The frame and tone come from the intake. The same policy can be framed around
cost, fairness, freedom, safety, or opportunity, and the right choice depends on
the candidate and the audience, not on a default. If no frame is provided, ask
which values the campaign wants to lead with before writing. Do not pick one
silently.

## Step 3: Build the explainer using this exact structure

```
# Policy explainer: [position], [candidate]

## Plain-English explanation
What the position is, in language a busy voter understands on first read. No
jargon. Lead with the frame from the intake.

## Why voters should care
The stakes for the voter's own life, tied to the frame.

## Local impact
What this means concretely in this district: a place, a number, a group of
people.

## Common objections
The real pushback this position will draw, stated fairly.

## Simple rebuttals
A short, honest answer to each objection. Concede what is fair, then make the
case.

## 30-second answer
What the candidate says when asked on the spot. One frame, one point, one proof.

## Website section
A headline and a few short paragraphs for the issues page.

## Door version
A sentence or two a canvasser can say at the door, in the frame from the intake.
```

Write the real copy for each, all in the same frame.

## Guidance

- **Plain beats clever.** If a voter has to reread it, rewrite it. Short
  sentences, concrete nouns, no insider terms.
- **Lead with the frame, then the facts.** Voters decide on values first and
  details second. The facts support the frame; they do not replace it.
- **Local makes it real.** A specific local impact lands harder than a national
  statistic.
- **Steelman the objection.** A rebuttal to a weak version of the objection
  convinces no one. Answer the strongest fair version.
- **Keep it honest.** Concede what is true, then argue. Overclaiming invites the
  rebuttal you cannot answer.

## References

- `references/intake.md`: fields to collect before writing the explainer.

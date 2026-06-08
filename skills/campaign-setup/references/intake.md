# Intake: fields to capture in the campaign profile

These are the shared fields stored in `campaigns/<name>.md` and reused by every
other skill in the pack. Gather them in a short conversation, one topic at a time.
Pull what you can from what the user has already said, ask for the rest, and leave
any field the user wants to skip clearly blank so they can fill it in later. Each
field notes what it drives downstream.

## Candidate and race

- **Candidate name.** Used throughout every skill and in bios, scripts, and
  releases.
- **Office sought.** Sets scope, formality, and which issues land (for example,
  School Board, State House District 14, Mayor).
- **District or jurisdiction.** Anchors local references and which races and issues
  are relevant.
- **Party (optional).** Drives the default tone and which contrasts are fair game.
  Leave out for nonpartisan or cross-partisan races.

## The contest

- **Opponent(s).** Used for persuasion contrast and rapid response, carefully and
  factually. Record "TBD" if it is not set yet.
- **Top three issues, in order.** The campaign's priorities. They key the messaging
  across every skill, so phrase them the way the campaign talks about them.

## Voice

- **Default tone.** One of professional, populist, or neighborly.
  - *Professional:* measured, informed, credible.
  - *Populist:* plain-spoken, us-versus-the-status-quo energy.
  - *Neighborly:* warm, local, first-name, "your neighbor" framing.
  - Individual skills can still stretch the tone for a given piece, but this sets
    the baseline.

## Key dates

- **Election date.** Drives GOTV, ballot chase, and any deadline-based messaging.
- **Early-vote window.** Start and end dates, where applicable. Drives the
  plan-to-vote sequences in field scripts.

## Notes (free text)

- **Anything else the skills should know** that does not fit a field: do-not-say
  language, a slogan or tagline, the values the candidate leads with, endorsements,
  or standing strategy notes. Skills check here before asking, so it is worth
  capturing.

These are working inputs the campaign owns and can edit by hand at any time. Keep
the file private; it is campaign-internal and should not go in a public repository.

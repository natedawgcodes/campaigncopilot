---
name: social-rapid-response
description: >-
  Turn a news item, press release, or opponent move into ready-to-post social
  content for a political campaign, fast. Use when a campaign or digital staffer
  needs to react on social media or repurpose a release into posts. Triggers on
  requests like "turn this news into posts", "rapid response to the opponent's
  statement", "make social posts from our press release", "give me a populist and
  a local version", or "we need a fundraising post off this story". Produces, per
  item, a professional version, a populist version, a local or community version,
  and a fundraising call-to-action version, with caption variations per platform.
  Reads references/intake.md first.
---

# Social Rapid Response

This skill converts a single news item or release into a set of posts a campaign
can publish immediately, in several voices and sized for each platform. Speed
matters in rapid response, so the output is post-ready, not a brief about posting.

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

Read `references/intake.md` to confirm the source item, the campaign's angle on
it, the platforms in use, the handles and hashtags, the link to include, the
donation link for the fundraising version, and any do-not-say constraints.

Collect what you can from the user's request and ask for the essentials that are
missing: the source item or its key facts, the campaign's take, and the platforms.
If the item is time-sensitive, draft from what you have and flag any gaps.

## Step 2: Lock the angle

Decide the one thing the campaign is saying about this item before writing.
Rapid response fails when posts wander. Every version below makes the same point
in a different voice; the angle is shared.

## Step 3: Build the posts using this exact structure

For the item, produce all four versions:

```
# Rapid response: [item]

## Professional version
Measured and credible. States the point with restraint. Suits official accounts.

## Populist version
Plain-spoken and direct, with energy. Names the stakes for regular people without
being performative.

## Local / community version
Grounds the point in this district: a local place, name, or impact. Sounds like a
neighbor, not a national account.

## Fundraising CTA version
The point plus a clear ask and the donation link. One reason to chip in now.
```

Then add platform caption variations:

```
## Platform variations
- X: short, one strong line, relevant handles and one or two hashtags.
- Facebook: a few sentences, room for context, link friendly.
- Instagram: caption for a graphic or photo, hashtags grouped at the end.
- Threads or short video caption: conversational, hook in the first line.
```

Write real captions. Keep each within the spirit of its platform's length and
norms, and respect the do-not-say list in every version.

## Guidance

- **Same angle, different voice.** The professional, populist, local, and
  fundraising versions are one message in four registers, not four messages.
- **Hook first.** The first line decides whether anyone reads the rest. Lead with
  it on every platform.
- **Local beats generic.** A specific street, school, or number outperforms a
  national talking point in district races.
- **Be fast but not loose.** Rapid response is quick, not careless. Do not
  overstate facts or repeat an opponent's framing while rebutting it.

## References

- `references/intake.md`: fields to collect before drafting posts.

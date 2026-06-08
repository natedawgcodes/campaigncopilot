# Intake: fields to collect before building the push

Gather these before writing. Pull what you can from the user's request, ask for
the essentials that are missing, and use clear placeholders for anything legal or
financial that the user must confirm. Each field is annotated with what it drives.

## Where these fields come from

If a `campaigns/<name>.md` profile exists, reuse the shared fields from it and do not
re-ask. Run the `campaign-setup` skill to create one if there is none.

- From the profile: candidate name, office, district or jurisdiction, party,
  opponent(s), top issues, default tone, and key dates (election date and early-vote
  window). The profile's notes section may also hold do-not-say language, a slogan,
  or endorsements.
- Ask per task (not stored in the profile): the reason to give now, the goal or
  deadline, what the money does, the audience (prior, lapsed, or new donors), the
  suggested amounts (ask ladder), the sender, the donation link, the required
  disclaimer text, and the SMS opt-in source.

The field notes below still apply; the profile simply pre-fills the shared ones.

## Candidate and ask

- **Candidate name and office.** Used throughout and in the sender voice.
- **The reason to give now.** The deadline, goal, match, or news moment that makes
  this ask urgent. This anchors every touch. Use the real reason; do not invent
  urgency.
- **Goal or deadline.** The number or date the push is built around. Drives the
  follow-up sequence escalation.
- **What the money does.** The concrete use of funds (for example, ads, field,
  voter contact). Makes the ask credible.

## Audience and ladder

- **Audience.** Prior donors, lapsed donors, or new prospects. Changes tone and
  the suggested amounts.
- **Suggested amounts (ask ladder).** The specific dollar options to offer. Drives
  the email ask and the donation-page call to action.
- **Sender.** Who the appeal is from (candidate, campaign manager, family member,
  surrogate). Sets the voice.
- **Tone.** Professional, populist, or neighborly.

## Logistics and compliance

- **Donation link.** The contribution URL the asks point to.
- **Required disclaimer text.** The paid-for or authorization line that must
  appear. The user supplies and confirms it; use a placeholder until then.
- **SMS opt-in source.** Where the texted recipients opted in. Relevant to opt-in
  awareness on the SMS version.

These compliance fields are awareness inputs, not legal advice. The user is
responsible for confirming disclaimers, contribution limits, and texting rules for
their own jurisdiction.

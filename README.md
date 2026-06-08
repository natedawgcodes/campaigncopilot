# Campaign Copilot

Campaign know-how, packaged as Claude skills your campaign can install once and run all cycle.

Campaign Copilot is a public pack of skills for the people who run political campaigns: field organizers, finance staff, comms leads, and the consultants who support them. Each skill turns a repeatable campaign task into an on-demand tool that drafts the work for you in seconds, in your candidate's voice.

## What is a skill, and how do I install it (60 seconds)

A skill is a folder with a `SKILL.md` file inside it. That file gives Claude step-by-step instructions and reference material for one specific job, like writing a canvass script. Claude reads the short description always, and loads the full instructions only when your request matches, so an installed skill costs almost nothing until you use it. You can let Claude pick the skill automatically from plain language, or run it directly by typing `/skill-name`.

### Install in Claude Code

Each skill is just a directory. Drop it into one of two places:

- `~/.claude/skills/<skill-name>/` makes it available across all your projects.
- `<your-project>/.claude/skills/<skill-name>/` scopes it to one project.

```bash
# clone this repo, then copy a skill into your personal skills folder
git clone https://github.com/natedawgcodes/campaigncopilot.git
cp -r campaigncopilot/skills/field-script-builder ~/.claude/skills/
```

Claude Code picks up the new folder within your current session. If `~/.claude/skills/` did not exist when you started, restart Claude Code once so it watches the new directory. Then ask in plain language, for example "write me a phone bank GOTV script for early voters," or invoke it directly:

```
/field-script-builder
```

### Install in claude.ai

Zip the skill folder and upload it under Settings, then Features. Custom skills are available on Pro, Max, Team, and Enterprise plans with code execution enabled.

### Good to know

- Every `SKILL.md` needs `name` and `description` in its YAML frontmatter. Names are lowercase with hyphens.
- Only use skills from sources you trust. Read what a skill does before you install it. Everything in this repo is plain text you can audit.

Full official docs: [Skills in Claude Code](https://code.claude.com/docs/en/skills) and [Agent Skills overview](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview).

## How to ask: a weak prompt vs a strong one

These skills reward specifics. The more of your role, race context, audience, tone, goal, and output format you give, the closer the first draft lands.

**Weak prompt**

> write a campaign email about taxes

The skill has to guess who you are, which race, who the email is for, what it should sound like, and what you want back. You get generic copy full of blanks.

**Strong prompt**

> Using `fundraising-generator`: I'm the finance director for Jane Miller, a Democrat challenging a two-term incumbent for Lakeside County Commission, District 3. Write an end-of-quarter fundraising email to past small-dollar donors in the district. Neighborly tone. The goal is to hit our June 30 filing deadline, built around Jane's property tax plan (a senior and longtime-homeowner exemption). Send me five subject lines, the main email with a suggested ask ladder, and a short resend for non-openers.

That one prompt carries role, race context, audience, tone, goal, and output format, so the draft comes back ready to edit instead of ready to redo. Better still, run `campaign-setup` once and the race context (candidate, office, district, opponent, issues, tone) is filled in for every skill automatically, so you only add what changes from task to task.

## Start here: set up your campaign once

Run `campaign-setup` before the other skills. It asks for your shared campaign context once (candidate, office, district, opponent, top issues, tone, and key dates) and saves it to a profile at `campaigns/<your-candidate>.md`. Every other skill reads that profile first, so you stop re-entering the same details for each script, release, or persona, and only answer the per-task questions that change from one job to the next.

Consultants running several races keep one file per campaign (for example, `campaigns/jane-miller.md` and `campaigns/sam-lee.md`), and the skills ask which campaign when there is more than one.

A note on privacy: the `campaigns/` folder holds campaign-internal information (opponent research, tone and strategy decisions, race notes). Do not commit it to a public repository. This repo ships a `.gitignore` that excludes `campaigns/` by default, but keep it in mind if you move the files or change your setup.

## The skills

Eleven skills across the departments a campaign actually runs, all built and ready to install today.

| Skill | What it does | Status |
| :--- | :--- | :--- |
| `campaign-setup` | Capture shared campaign context once into a profile the other skills read first | Built |
| `field-script-builder` | Voter-contact scripts for door, phone, and SMS across voter ID, persuasion, GOTV, volunteer recruitment, and ballot chase | Built |
| `voter-persona-builder` | Define target voter segments and match a tailored message to each | Built |
| `oppo-research-organizer` | Organize public, user-provided info into a structured vulnerability memo | Built |
| `debate-prep-coach` | Debate prep: likely and hostile questions, answers, bridges, and a closing | Built |
| `candidate-message-builder` | One disciplined message set across stump, bio, palm card, SMS, and social | Built |
| `fundraising-generator` | A multi-touch donor ask across email, SMS, and the donation page | Built |
| `press-release-writer` | Full releases by type, plus reporter pitch and social copy | Built |
| `social-rapid-response` | Turn a news item into posts in several voices, sized per platform | Built |
| `policy-explainer` | Turn a policy position into plain, voter-ready language | Built |
| `website-copy-builder` | Page-by-page campaign website copy with form fields and SEO | Built |

## Can't run skills, or want it done for you

Not every campaign has someone set up to run Claude, and that is fine. If you want these built into your program, a custom skill for a workflow that is specific to your race, or a done-for-you package, reach out:

- Email: nathan@victoryframeworks.com
- Web: campaigncopilot.dev

Tell us the office, the jurisdiction, and the task you keep redoing by hand, and we will point you at the right skill or build the one you need.

## License

Apache 2.0. See [LICENSE](LICENSE).

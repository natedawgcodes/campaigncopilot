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

## The skills

Ten skills planned across the departments a campaign actually runs. One is built and ready to install today; the rest are on the way.

| Skill | What it does | Status |
| :--- | :--- | :--- |
| `field-script-builder` | Voter-contact scripts for door, phone, and SMS across voter ID, persuasion, GOTV, volunteer recruitment, and ballot chase | Built |
| `fundraising-appeal-writer` | Donor emails, text appeals, and call-time scripts tuned to ask amount and audience | Planned |
| `press-release-builder` | Press releases, media advisories, and rapid-response statements | Planned |
| `stump-speech-writer` | Stump speeches and talking points in the candidate's voice | Planned |
| `gotv-planner` | Get-out-the-vote turnout plans, shift goals, and chase lists for the final stretch | Planned |
| `volunteer-recruiter` | Recruitment funnels, sign-up asks, and first-shift onboarding | Planned |
| `social-content-pack` | Platform-ready social posts and a week-at-a-glance content calendar | Planned |
| `targeting-memo-builder` | Turn a voter universe into a written targeting and contact plan | Planned |
| `debate-prep-kit` | Debate prep, mock questions, pivots, and rapid-response lines | Planned |
| `endorsement-outreach` | Endorsement requests and follow-ups to organizations and local leaders | Planned |

## Can't run skills, or want it done for you

Not every campaign has someone set up to run Claude, and that is fine. If you want these built into your program, a custom skill for a workflow that is specific to your race, or a done-for-you package, reach out:

- Email: hello@campaigncopilot.dev
- Web: campaigncopilot.dev

Tell us the office, the jurisdiction, and the task you keep redoing by hand, and we will point you at the right skill or build the one you need.

## License

MIT. See [LICENSE](LICENSE).

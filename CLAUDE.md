# Campaign Copilot

This repository is a pack of Claude skills for political campaign staff and
consultants. Each skill packages campaign know-how into a repeatable, on-demand
tool. The pack is distributed publicly through this repo so campaigns can install
and run the skills themselves. A separate landing page lives at campaigncopilot.dev.

## Conventions

These hold for every file in the repo, including this one.

- No em dashes anywhere, in any file. Use periods, commas, parentheses, colons,
  or the word "to" for ranges (for example, "1 to 5").
- No AI or Anthropic attribution anywhere. Not in commit messages, not in code
  comments, not in any file content. Commits must not include a Co-Authored-By
  trailer or a "Generated with" line. Referring to the Claude product where a
  user installs a skill is fine; crediting authorship to an AI is not.
- Commit messages: lowercase, 5 to 8 words, no body.
- File edits and git operations are handled in this workflow. Branch merges are
  run by the maintainer in the terminal.

## Repository structure

```
skills/<skill-name>/
  SKILL.md            # the skill entrypoint (required)
  references/         # supporting material the skill loads on demand
README.md             # landing page, install guide, and skill index
LICENSE               # MIT
CLAUDE.md             # this file
```

## Writing skills here

- Every SKILL.md needs YAML frontmatter with `name` and `description`. Keep the
  name lowercase with hyphens, and never use words that platforms reserve
  (for example, the product or company names).
- Put trigger phrasing in the `description` so the skill loads when a campaign
  user asks in plain language, not only when they type the command.
- Keep SKILL.md focused. Move long reference material into `references/` and
  point to it from the body so it loads only when needed.
- Treat compliance content as operational awareness, not legal advice. Every
  skill that touches voter contact reminds the user to confirm the rules for
  their own jurisdiction.
- Match the voice a campaign staffer would actually use: plain, direct, and
  ready to run in the field.

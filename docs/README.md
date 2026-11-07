# Chat home

Open new Cursor chats on [cfwest86/cfwest86](https://github.com/cfwest86/cfwest86).

This repository is a directory. It tells the agent which other repository to use, or asks you before a new one is created. Project code stays in those other repositories.

The root `README.md` is the public GitHub profile and is separate from this guide.

## What the agent reads

| File | Role |
| --- | --- |
| `AGENTS.md` | Instructions applied to every chat opened here |
| `.cursor/rules/home-base.mdc` | Always-on rule: route work, keep this repo a directory |
| `.cursor/rules/catalog.mdc` | Applied while editing files in `docs/` |
| `.cursor/skills/route-chat/` | Pick an existing repo, this repo, or a new repo |
| `.cursor/skills/propose-new-repo/` | Draft a new repository and the first prompt for it |
| `.cursor/skills/update-repo-catalog/` | Record a repository after it exists |
| `docs/repos.md` | The catalog of repositories |

## What to say when you open a chat

Describe the outcome you want. You do not need to name a repository.

Examples:

- "Add a chart of Florida home values over the last 20 years."
- "Continue the school district Jupyter analysis and explain the bottom five schools."
- "I need a new private repo for a client pricing workbook."

The agent reads the catalog and answers with one of three results:

1. **Stay here** for changes to the rules, skills, or catalog.
2. **Open the next chat in an existing repo**, with a link and a prompt you can paste.
3. **Propose a new repo**, with a name, visibility, and a starter prompt. Nothing is created until you say yes.

## After a new repository exists

Tell the agent the GitHub URL. It adds the repository under Active in `docs/repos.md` so the next chat can find it.

## Visibility

This repository is public. Keep secrets and private notes out of it. Prefer a private repository for new work unless you want it on your public profile.

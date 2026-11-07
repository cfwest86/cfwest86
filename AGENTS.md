# Home base

This repository is where new chats start. It holds the rules, skills, and catalog that send work to the right GitHub repository.

`README.md` is the public GitHub profile. Leave that profile text in place. Hub docs live in `docs/`.

## Start of every chat

1. Read `docs/repos.md`.
2. Decide where the work belongs.
3. Say that decision before editing anything.

| The request is about | Where it goes |
| --- | --- |
| Rules, skills, the catalog, or how chats are routed | This repository |
| A repository already listed in `docs/repos.md` | That repository. Stop here and hand off a prompt. |
| New work with no matching repository | A new repository. Propose it and wait for a yes. |

Use the `route-chat` skill for that decision. Use `propose-new-repo` when nothing in the catalog fits. Use `update-repo-catalog` after a repository is created, renamed, or archived.

## What stays out of this repository

- Application code, notebooks, and data for a specific project
- Secrets, tokens, credentials, and private personal data

This repository is public. Anything committed here is visible on GitHub.

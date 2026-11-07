---
name: update-repo-catalog
description: Add or revise an entry in docs/repos.md. Use after a repository is created, renamed, archived, or when its purpose changes.
---

# Update the repository catalog

Edit `docs/repos.md` only. Do not copy the repository list into rules or skills.

## Add an active repository

Put a new `### repo-name` block under `Active`. Once the first active repository exists, remove the line that says there are none. Leave the entry template in place below the real entries.

Required fields:

| Field | What to write |
| --- | --- |
| URL | `https://github.com/cfwest86/<repo-name>` |
| Status | `active` |
| Purpose | One sentence a future chat can match a request against |
| Open a chat here when | The kinds of requests that belong there |

Confirm the repository exists before adding it. A proposal is not an entry.

## Other changes

- **Archive:** move the entry out of Active. Add one row to the Archive table with the repo link and a short "what it is". Delete the Active block.
- **Rename or new purpose:** replace the name, URL, and purpose. Keep the old name out of Active so chats do not route to a missing repository.
- **Refresh:** when the user asks to rescan GitHub, compare the account's repositories with this file, add missing ones, and set `Catalog checked` to today's date.

Leave the root `README.md` profile text unchanged unless the user asks to change the GitHub profile.

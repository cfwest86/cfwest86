---
name: propose-new-repo
description: Propose a new GitHub repository when the catalog has no match. Use when the user wants a new project or codebase, or when route-chat finds no home. Drafts the name, visibility, catalog row, and starter prompt. Does not create the repository.
---

# Propose a new repository

Confirm `docs/repos.md` has no matching Active or named Archive repository. If one matches, use `route-chat` instead.

Creating the GitHub repository waits for an explicit yes. Do not add project files to this home repository in the meantime.

## Draft

Propose one repository:

- **Name:** lowercase, hyphenated, under the `cfwest86` account. Derive it from the work, not from a generic word like `project` or `new-repo`.
- **Description:** one sentence that can later be pasted into the catalog as the purpose.
- **Visibility:** private. Switch to public only when the user says the work belongs on their public profile or is a portfolio piece.
- **First chat:** what the first session in the new repository should accomplish.

Show a catalog row in the Active format from `docs/repos.md`, ready for `update-repo-catalog` once the URL exists.

Then show a starter prompt:

```markdown
You are in cfwest86/<repo-name>.

Goal: <one sentence>.

Done when: <observable outcome>.

Constraints: <only the constraints the user already gave>.
```

## After the user says yes

Ask them to create an empty repository with that name and visibility, then open a new Cursor chat on it and paste the starter prompt.

When they send the URL, use `update-repo-catalog` to add the Active entry. Until that URL exists, leave the catalog unchanged.

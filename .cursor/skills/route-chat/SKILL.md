---
name: route-chat
description: Decide whether work stays in this home repo, moves to a listed repo, or needs a new repo. Use at the start of a chat that asks for project work, a codebase change, analysis, or where something should live.
---

# Route a chat

Read `docs/repos.md` before choosing. The catalog is the source of truth.

## Decide

1. **Stay here** when the user wants to change rules, skills, the catalog, or the way chats are routed. Do that work in this repository.
2. **Hand off** when an Active repository's purpose matches the request, or when the user names an Archive repository (or is clearly continuing that coursework). Do the project work in that other repository.
3. **Propose a new repository** when no entry matches. Follow the `propose-new-repo` skill. Do not start the project in this repository while you wait.

If two repositories could match, name both and ask which one to open. Ask that one question before writing a handoff prompt.

## Hand off

Stop editing. Reply with:

1. The repository name and URL.
2. One sentence on why it matches.
3. A prompt the user can paste into a new chat opened on that repository. Include the goal, the constraints they already gave, and the files or data they mentioned. Leave out hub-routing instructions.

Use this shape:

```markdown
Open the next chat in [repo-name](https://github.com/cfwest86/repo-name).

Why: one sentence.

Paste this:

> The prompt, in the user's words, with the details they already provided.
```

Archive matches need a reminder that the repository is older coursework, then the same handoff.

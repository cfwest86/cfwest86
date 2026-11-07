---
name: create-repo
description: Create a new GitHub repository for a project that is not in the catalog. Use when the user asks for a new repo, a new project, or a place to keep work that does not belong in an existing repository.
---

# Create a repository

1. Read `repos/catalog.md` and confirm the work does not belong in an existing repository.
2. Choose a short name: lowercase letters, numbers, and hyphens. Prefer a name that says what the project is.
3. Create it as a private repository owned by `cfwest86`:

```bash
gh repo create cfwest86/<name> --private --description "<one line>" --add-readme
```

4. If GitHub returns `createRepository` or `Resource not accessible by integration`, stop. Tell Carson the repository name and the command above. Do not scaffold the new project inside this home.
5. When the repository exists and is in the environment, add a row to `repos/catalog.md` with the name, a one-line topic, and the URL.
6. In the new repository, add a `README.md` that states what the project is and an `AGENTS.md` only when the project needs instructions beyond the home rules.

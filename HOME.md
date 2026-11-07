# Agent home

This repository is the home for Cursor skills, rules, and the catalog of project repositories. Agents opened here use these files to decide where work belongs and when a new repository is needed.

The profile `README.md` is the GitHub profile page. Leave it as it is unless Carson asks to change that page.

## What belongs here

- Agent instructions in `AGENTS.md`
- Rules in `.cursor/rules`
- Skills in `.cursor/skills`
- The project catalog in `repos/catalog.md`

Project code, notebooks, data, and new products belong in their own repositories.

## How routing works

1. Read `repos/catalog.md`.
2. If the request matches an existing project, that repository is where the work goes.
3. An agent can change a project repository only when that repository is part of the same cloud environment. Otherwise the next agent has to be started with that repository included.
4. If no existing project fits, follow the create-repo skill and make a new repository.

## Creating a repository

This session can push to `cfwest86/cfwest86`. It cannot create a new GitHub repository: the token returns `Resource not accessible by integration (createRepository)`.

When that happens, create the empty repository from the GitHub account, add it to the cloud environment, and start the next agent there. Then add a row to `repos/catalog.md`.

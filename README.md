# MonoProjects

MonoProjects is a personal monorepo that collects projects, prototypes, libraries, and ideas. It’s a place to experiment, share small apps, and maintain reusable packages.

## Purpose
- Keep runnable applications and reusable libraries together for easy discovery and reuse.

## Repository layout
- `apps/` — runnable applications; each app lives in its own subfolder with its own README and run instructions.
- `packages/` — reusable libraries, components, or tools intended for sharing across apps.

## Matt Pocock agent skill

This repository includes Matt Pocock’s [`setup-matt-pocock-skills`](.agents/skills/setup-matt-pocock-skills/SKILL.md) skill. It configures repo-specific guidance for issue tracking, triage labels (when the triage skill is installed), and domain documentation.

Run it once from this repository in a coding agent that supports Agent Skills:

```text
/setup-matt-pocock-skills
```

Review and confirm the proposed setup before it writes files. The skill detects this repo’s GitHub remote and recommends GitHub Issues for tracking; it also checks for monorepo structure when suggesting a domain-doc layout. Setup files are written under `docs/agents/`, with a short pointer added to the existing `AGENTS.md` or `CLAUDE.md` (if present). Commit the generated configuration so it is shared with the repo. See the [upstream skills repository](https://github.com/mattpocock/skills) for the full collection and installation/update instructions.

## Adding a project
1. Create a directory under `apps/` or `packages/`.
2. Add a README with purpose and usage.
3. Add tests or build scripts when applicable.
4. Open a PR and describe the project in the PR description.

## Examples
- `apps/example-app/` — a minimal app demonstrating conventions.
- `packages/example-lib/` — a small reusable library.

## Contributing
- Open an issue to discuss larger changes.
- Follow repository conventions in PRs: README, tests, and a short description.

## License
Where applicable, packages include their own license files. If the repository gains a top-level license, it will be noted here.

## Contact
Maintained by the repo owner. Open issues or PRs for questions or contributions.

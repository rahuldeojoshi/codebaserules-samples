# CodebaseRules: free samples

Free sample rule files from the paid [CodebaseRules](https://codebaserules.com) packs for **Cursor** and **Claude Code**. Each paid pack teaches your AI coding assistant the conventions for one stack, such as layering, error handling, persistence, security, testing, and naming, so that generated code matches how the codebase is meant to look.

This repo contains **two real rule files from each pack**:

| Stack | Sample files |
|---|---|
| FastAPI + Python 3.12 | `10-routers-schemas.mdc`, `30-database.mdc` |
| Next.js 15 App Router + TypeScript | `10-routing-components.mdc`, `20-server-actions-errors.mdc` |
| Spring Boot | `20-errors.mdc`, `30-persistence.mdc` |

## Install in Cursor

Copy the `.mdc` files for your stack into your project's `.cursor/rules/` directory:

```bash
mkdir -p .cursor/rules
cp fastapi/.cursor/rules/*.mdc /path/to/your-project/.cursor/rules/
```

Each rule has `globs` in its frontmatter. Cursor attaches a rule automatically when you edit a file that matches those globs.

## Use with Claude Code

Claude Code reads project instructions from `CLAUDE.md` at the repo root. The samples ship only as Cursor `.mdc` files. To use one with Claude Code, paste the rule body (the part below the frontmatter) into your `CLAUDE.md`. The full packs include a ready-made `CLAUDE.md` for each stack.

## Full packs

The complete packs (FastAPI, Next.js, Spring Boot) contain the full rule set plus `CLAUDE.md`.

Want to know what changed in AI coding tools? See the **[AI coding changelog](https://changelogs.codebaserules.com)**.

## License

MIT. See [LICENSE](LICENSE). This license covers only the sample files in this repo.

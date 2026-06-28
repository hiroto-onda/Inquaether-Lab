# Development Notes

## 1. Purpose

This file records current development and operations notes for Inquaether Lab so future work does not depend on memory or prior chat context.

It is documentation only. It does not define automation, scripts, scheduled tasks, or source repository behavior.

## 2. Repository Role

`Inquaether-Lab` is primarily a public website, documentation, and application-planning repository.

Use this repository for:

- Public-facing website content.
- Documentation and research-facing notes.
- Application planning materials.
- Local support notes for evidence gathering.

Do not treat this repository as the source of truth for implementation work in related repositories unless explicitly requested.

## 3. Local Repository Location

The local repository root is:

```text
/Users/ondahiroto/Documents/Inquaether-Lab
```

All repository-relative paths in this file assume that root.

## 4. GitHub Pages Notes

GitHub Pages is served from the repository content.

Current public-site files include:

- `index.html`
- `404.html`
- `robots.txt`
- `sitemap.xml`
- `assets/`

Do not change GitHub Pages settings unless explicitly requested.

For documentation-only operations, do not modify:

- `index.html`
- `README.md`
- `docs/`
- `applications/`
- `assets/`
- GitHub Pages settings

## 5. Python / Virtual Environment Notes

The Python virtual environment is not inside `Inquaether-Lab`.

The current Python virtual environment is located at:

```text
/Users/ondahiroto/Documents/lumenia-exogram/.venv314
```

To activate it:

```sh
cd /Users/ondahiroto/Documents/lumenia-exogram
source .venv314/bin/activate
```

Do not create a new virtual environment inside `Inquaether-Lab` unless explicitly requested.

## 6. Related Repositories

Related repositories include:

- `ci_theory`
- `lumenia-exogram`
- `Inquaether-Lab`

Current rule: do not write to `ci_theory` or `lumenia-exogram` unless explicitly requested later.

When related repositories are used as sources, treat them as read-only evidence sources by default.

## 7. Research Memory OS Notes

Research Memory OS v0 is located under:

```text
applications/longview_digital_minds_2026/research_memory_os_v0/
```

Research Memory OS v0 is manual, read-only, and evidence-gathering focused.

Research Memory OS v2 is currently design-note only. It should not be treated as implemented infrastructure.

Current rule:

- No automation.
- No scripts.
- No API usage.
- No scheduled tasks.
- Read-only source handling.
- No writes to `ci_theory` or `lumenia-exogram` unless explicitly requested later.

## 8. Codex Usage Rules

Codex should:

- Keep work scoped to the user request.
- Preserve existing repository boundaries.
- Show diffs before committing.
- Stop before committing unless the user explicitly asks for a commit.
- Avoid creating scripts, automations, scheduled tasks, or API workflows unless explicitly requested.
- Treat source repositories as read-only when gathering application evidence.

Codex should not rely on memory as the only place where project rules live. Durable operating notes should be written into repository documentation when requested.

## 9. Git Workflow

Default workflow:

1. Inspect the current repository state.
2. Make the requested documentation or code change only.
3. Show the diff.
4. Stop before committing.

Do not stage, commit, push, or open pull requests unless explicitly requested.

Avoid broad refactors or unrelated edits during documentation-only tasks.

## 10. Safety Boundaries

Current safety boundaries:

- Do not modify existing `ci-memory-weekly-sync` automation.
- Do not create new automation.
- Do not create scripts.
- Do not use APIs for Research Memory OS v0.
- Do not create scheduled tasks.
- Do not modify `ci_theory` or `lumenia-exogram` unless explicitly requested later.
- Do not modify `README.md`, `index.html`, `docs/`, `applications/`, `assets/`, or GitHub Pages settings during documentation-only root-note updates.
- Keep source handling read-only and evidence-focused.
- Keep generated summaries separate from primary source evidence.

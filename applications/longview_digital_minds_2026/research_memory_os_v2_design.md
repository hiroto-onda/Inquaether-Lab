# Research Memory OS v2 Design Note
Status: Design Note Only

## Purpose

Research Memory OS v2 is a future design for a lightweight research-memory layer that helps gather, index, and summarize scattered research context without changing source repositories or existing automations.

The intended use is to support fellowship applications, research handoffs, and periodic self-review by producing evidence-bound summaries from approved read-only sources.

## Non-Goals

- Do not modify the existing `ci-memory-weekly-sync` automation.
- Do not modify `ci_theory`.
- Do not modify `lumenia-exogram`.
- Do not create a new automation.
- Do not write to any source repository.
- Do not replace human review, judgment, or final application writing.
- Do not infer research claims beyond observed source material.

## Safety Boundaries

- Treat all connected sources as read-only unless a separate, explicit write request is made later.
- Keep generated summaries clearly separated from primary research evidence.
- Preserve source attribution for every claim that may be reused in public writing.
- Mark uncertain, incomplete, or conflicting evidence instead of smoothing it over.
- Avoid background sync behavior, hidden scheduled tasks, or unattended edits.
- Keep this design isolated from current CI memory workflows.

## Cost Limit

The operating budget must remain under 3,000 JPY per month.

Cost controls should include:

- Manual runs only in the v0 workflow.
- Small source batches instead of full-archive scans.
- Local text indexing where practical.
- Explicit limits on model calls, file counts, and token volume.
- No paid external services unless their monthly cost is already known and fits inside the cap.

## Read-Only Policy

Research Memory OS v2 should read from approved sources and produce local design outputs or draft notes only inside this application workspace.

It must not:

- Commit, push, or rewrite Git history.
- Edit source repositories.
- Run repository sync scripts.
- Modify existing automation configuration.
- Create calendar, reminder, or background automation entries.
- Upload generated material back to Google Drive or GitHub without a later explicit write request.

## Source Candidates

- GitHub repositories and issues, read through authenticated or public read-only access.
- Google Drive documents, spreadsheets, PDFs, and exported text, read through explicit user-selected files or folders.
- ChatGPT exports, read from local export files selected by the user.
- Note drafts, read from local Markdown, text, or document files in the application workspace.

## v0 Minimal Workflow

1. The user selects a small source set for one research question or application section.
2. The system reads only those selected files or links.
3. The system extracts candidate evidence snippets with source labels.
4. The system groups evidence by theme, uncertainty, and possible application relevance.
5. The system produces a local Markdown brief in the application workspace.
6. The user reviews the brief and manually decides what to reuse.

The v0 workflow should be command-driven and manual. It should not run on a schedule, watch folders, or update any repository automatically.

## Risks

- Accidental scope creep into automation or repository maintenance.
- Mixing generated summaries with primary evidence.
- Overstating claims from incomplete or stale source material.
- Cost growth from broad scans or repeated model calls.
- Privacy risk from reading sensitive personal notes or exports.
- Connector permission drift if future tools gain write access by default.
- Confusion with the existing CI weekly memory workflow.

## Future Upgrade Path

- Add a source manifest that records approved read-only locations and exclusion rules.
- Add a local evidence index with source hashes, timestamps, and provenance metadata.
- Add repeatable brief templates for applications, research retrospectives, and handoff notes.
- Add a budget meter that estimates monthly model and connector costs before each run.
- Add a review queue for claims that need stronger citation or human confirmation.
- Add optional export formats only after the read-only v0 workflow is stable.
- Revisit automation only in a separate design review with explicit safety, cost, and write-permission controls.

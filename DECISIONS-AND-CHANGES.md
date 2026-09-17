# Decisions and changes

[Home](README.md)

## Document status

This v0.1.0 handbook is a review draft assembled on 2026-09-17. The individual seed rules restate prior project requests, but their exact cross-project wording needs review. No general handbook approval has been recorded.

## Proposed governance

**Status:** Proposed, not a previously approved user policy.

Keep shared rules in one canonical place. Adopt a named handbook version in each project brief, rather than silently forcing every existing product onto the latest draft. A handbook update does not automatically authorize a source-code migration.

Use these statuses:

| Status | Meaning |
| --- | --- |
| Seeded / review draft | Based on existing context, but the consolidated wording and scope still need review. |
| Proposed | A new recommendation, not a binding requirement. |
| Approved | Explicitly accepted by Will, with the approval/date recorded. |
| Superseded | Replaced by an identified later decision; retained for history. |

Do not convert an AI recommendation, silence, or an unreviewed generated file into an approval record.

## Suggested maintenance habit

At the end of meaningful work, extract only decisions and recurring lessons. For each, ask whether it belongs to a single project, a conditional module, or the universal baseline. Update the affected page after review, log the change, and refresh any handoff snapshot before the next use.

This should be one small update, not a full transcription of the chat. A renamed button usually belongs in the project brief; a repeated import-contract failure may justify a conditional standard.

## Change proposal template

### [CHANGE-ID] — [Title]

Status: Proposed
Date: [Date]
Affected page/rule: [File + ID]
Scope: Universal / Conditional module / One project
Source of lesson: [Actual task, user statement, artifact, or test]
Proposed wording: [Exact replacement or addition]
Reason: [What failure or ambiguity this prevents]
Conflicts/exceptions: [Known conflicts or none identified]
Affected projects: [Candidates, not automatic migration orders]
Verification: [How compliance can be checked]
Approval: [Pending until explicitly accepted]

## Initial changelog

| Version | Date | Change | Approval status |
| --- | --- | --- | --- |
| v0.1.0 | 2026-09-17 | Created the linked Markdown starter, seeded rule boundaries, product-role map, handoff prompts, template, and checklist. | Review draft; not ratified. |

## Not yet decided

The final scope/wording of the universal baseline; which project will trial it first; whether GitHub is selected as the canonical home; and whether a later automated handoff/export workflow is worth adding.

A proposed shared evidence schema, automatic synchronization, and integration rewrites are deliberately out of scope for this starter.

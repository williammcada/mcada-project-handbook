# Decisions and changes

[Home](README.md)

## Document status

This handbook began as a v0.1.0 review draft assembled on 2026-09-17. The current canonical baseline is v0.1.3 (2026-10-01). U-09 and U-10 are approved requirements; U-01–U-08 retain their seeded/review status. No general approval of the remaining draft handbook has been recorded.

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

The final scope/wording of the remaining seeded universal baseline; which project will trial those seeded rules first; and whether a later automated handoff/export workflow is worth adding. GitHub is the canonical home, as recorded in the approved amendments below.

A proposed shared evidence schema, automatic synchronization, and integration rewrites are deliberately out of scope for this starter.

## Approved amendment — U-09 (2026-09-29)

William McAda explicitly requested school-year deletion and clearing saved benchmarks, and instructed that this become a universal GitHub rule for every project going forward. U-09 in UNIVERSAL-RULES.md is approved; the prior seeded rules retain their original status. Added corresponding project-template and release-checklist entries. No conflict with U-06: deliberate owner-confirmed deletion is distinct from accidental feature/data loss. Benchmark Studio v0.3.1 implements the rule; other existing applications have not been modified by this amendment. GitHub remains the canonical handbook; older downloaded snapshots are historical exports.

## Approved amendment — U-10 (2026-10-01)

William McAda reported a stuck D-pad while playing the first MathQuest side-scrolling shooter candidate and explicitly requested a universal rule to double-check touchscreen controls. U-10 records that requirement with concrete interruption, cancellation and multi-touch regression checks, including real-device evidence. Added a release-checklist row. The rule applies wherever held controls exist; it does not authorize or claim a completed migration of other applications. U-01–U-08 retain their seeded status. No conflicting rule was identified.

## Approved U-10 reinforcement and MathQuest timing — 2026-10-01

The owner reported recurring stuck controls in aerial practice v0.1.1 and supplied an iPhone Edge screenshot with HULL text selected and the Copy/Search/Ask Copilot/Translate/Look Up menu open. He explicitly requested these recurring issues in the universal GitHub rules. U-10 now includes the entire gameplay surface, native text-selection/callout prevention, native contact-list reconciliation, shared implementation, and hosted/standalone regression checks. This strengthens the existing approved rule rather than introducing a parallel rule. It does not claim every historical game or physical device has been repaired.

The same instruction increased the aerial level from three to five active minutes, doubled its regular enemies, and increased player movement speed by 10%. S-03-A records five minutes as the MathQuest action-minigame default. Enemy quantity and movement tuning remain local to this aerial revision. Existing cartridge migrations retain explicit scope; unrelated game settings and curriculum standards are preserved.

## U-10 clarification — mobile zoom, viewport and native menus (v0.1.3, 2026-10-01)

**Status:** Clarification of the approved U-10 requirement, requested by William McAda on 2026-10-01 (Asia/Shanghai).

The owner asked to confirm and specify universal GitHub coverage for recurring locked controls, random zooming in/out and the iPhone context menu previously reported in the aerial shooter. The canonical v0.1.2 pages already covered stuck controls, native selection/callouts and gesture zoom. This amendment makes viewport stability and its verification explicit rather than creating a separate competing rule.

U-10 now distinguishes the three concerns, specifies stable gameplay through browser-bar/orientation/keyboard changes, and requires separate evidence for input release, viewport behavior and native-menu prevention. Disruptive failures block release on affected supported devices. Physical-device checks still required are marked Not run; synthetic events or desktop emulation must not be described as physical iPhone/iPad verification. PROJECT-TEMPLATE.md and RELEASE-CHECKLIST.md carry the requirements into future work. README.md advances to v0.1.3.

**Scope/conflicts:** New games and revisions of existing games on their declared target devices; held-control handling also applies to other projects using held input. Ordinary settings/forms, scrolling, copying and accessible zoom outside gameplay remain usable. No conflict with U-05/U-07/U-08 was identified. This documentation change does not audit, modify or certify any game implementation. Prior combined upload snapshots are historical copies; no combined snapshot is tracked in this repository.

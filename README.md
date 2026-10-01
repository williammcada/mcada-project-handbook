# William McAda — Project Handbook

**Version:** v0.1.3 · **Date:** 2026-10-01 · **Status:** U-09 and U-10 approved; earlier seeded rules remain review drafts

A shared reference for the rules, vocabulary, and decisions that should carry between projects. This is not another application, a source-code repository for the games, or an archive of every conversation.

## Start with these three pages

1. [Universal rules](UNIVERSAL-RULES.md): review which expectations really belong across the product family.
2. [Project map](PROJECT-MAP.md): check each product's purpose and which conditional standards fit it.
3. [AI handoff](AI-START-HERE.md): use this at the beginning and end of development work.

## All pages

| Page | Purpose |
| --- | --- |
| [Universal rules](UNIVERSAL-RULES.md) | Shared quality expectations, with scope boundaries and checks. |
| [Conditional standards](CONDITIONAL-STANDARDS.md) | Extra rules activated by a project's features or audience. |
| [Project map](PROJECT-MAP.md) | Product roles, relationships, and exceptions. |
| [Glossary](GLOSSARY.md) | Shared meanings without forcing shared implementation. |
| [Project template](PROJECT-TEMPLATE.md) | A short, project-specific brief to copy and complete. |
| [AI handoff](AI-START-HERE.md) | Reading instructions and reusable opening/closing prompts. |
| [Release checklist](RELEASE-CHECKLIST.md) | Evidence-oriented checks for each delivery. |
| [Decisions and changes](DECISIONS-AND-CHANGES.md) | Rule status, amendments, and a change proposal template. |
| [References](REFERENCES.md) | Setup documentation and the limits of this consolidation. |

## What this draft does—and does not—establish

The seed rules restate preferences and lessons from prior project discussions. Their exact wording and global scope are a **draft consolidation**, not a claim that Will approved every sentence. Proposed governance procedures are separately labeled. Review the rules before declaring an approved baseline.

No application source code was inspected for this handbook. Project descriptions capture intended roles, not verified implementation or the latest release numbers. Do not treat an item in the handbook as evidence that a product already implements it.

## Start using it

Extract the ZIP. Keep the files together and open `README.md`. For a first trial, review the universal rules, copy the project template into a named project brief, and provide the handbook plus that brief and the actual current source package to the AI doing the work.

The separately supplied `McAda_AI_Context_v0.1.0.md` is a combined, read-only snapshot of these pages for convenient AI upload. Edit the individual source pages, not both versions. After changes, regenerate the combined snapshot before reusing it.

## Put the handbook on GitHub

Suggested repository name: `mcada-project-handbook`. Start with a **private** repository. Upload the extracted Markdown files—not the unopened ZIP—to the repository's Code area. An empty repository offers an “uploading an existing file” link; an initialized repository has **Add file → Upload files**. Keep `README.md` at the root. GitHub renders it and its relative links as a navigable handbook. [Setup references](REFERENCES.md)

There is no deployment step, Pages site, Actions workflow, hidden folder, or build dependency in this package.

Once uploaded, choose GitHub as the master copy. Edit pages there and commit meaningful changes. Treat downloaded copies and AI context snapshots as dated exports. Do not independently edit several copies and assume they synchronize.

Obsidian is an optional local reading/editing interface: open the extracted folder with **Open folder as vault**. No automatic synchronization is configured by this package. [Obsidian reference](REFERENCES.md)

## Keep the process small

Start with one active project. Do not import all historic chats. Bring forward decisions, constraints, recurring failure modes, and current facts. Add more project briefs only when needed. The goal is less repeated explanation, not another administration job.

## Approved saved-work management rule

[U-09](UNIVERSAL-RULES.md#u-09--let-users-delete-saved-work-and-start-fresh) requires individual/group deletion and clear-all controls in projects with saved work. Approved by Will on 2026-09-29; see the decisions log. Existing applications still need implementation when revised. Older v0.1.0 combined snapshots predate this rule; use these canonical pages.

## Approved held-control reliability rule

[U-10](UNIVERSAL-RULES.md#u-10--prevent-stuck-controls-and-verify-touch-release) requires explicit stuck-control regression checks, multi-touch and interruption handling, and real target-device evidence. Requested by Will on 2026-10-01. Existing applications require individual audits when revised; this amendment does not claim their controls are already fixed.

## iPhone control reinforcement and MathQuest timing

The 2026-10-01 [U-10 amendment](UNIVERSAL-RULES.md#u-10--prevent-stuck-controls-and-verify-touch-release) also covers native text-selection/callout menus and one tested input mechanism across each codebase. [S-03-A](CONDITIONAL-STANDARDS.md#s-03-a--mathquest-action-minigame-timing) records the approved five-minute MathQuest action default. These are requirements for implementation and verification, not claims that all older games already comply.

## Explicit mobile gameplay checks — v0.1.3

[U-10](UNIVERSAL-RULES.md#u-10--prevent-stuck-controls-and-verify-touch-release) now specifies three recurring concerns separately: stuck input, unintended browser zoom/layout movement, and native selection/context menus. The project template and release checklist carry these checks forward, including rotation, browser bars, software keyboards and physical-device evidence. These are universal requirements where applicable; saving them does not certify or repair existing games.

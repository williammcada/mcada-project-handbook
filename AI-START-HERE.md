# AI handoff

[Home](README.md) · [Project template](PROJECT-TEMPLATE.md) · [Release checklist](RELEASE-CHECKLIST.md)

**Status:** Proposed working procedure. Use it explicitly for a task; the filename does not make an AI load or obey it automatically.

## What to provide at the beginning

Provide the universal rules, selected conditional standards, project brief, and release checklist, together with the actual current source artifact and any specification the task depends on. The companion combined Markdown snapshot is a convenient way to supply the shared handbook in one file.

Use the project map and glossary when architecture or terminology matters. Do not make the AI reconstruct current implementation from a project-role summary.

Files attached to a past chat, local links, and a private repository address must not be assumed accessible in a new session. Use files actually supplied to that session, or an authorized retrieval integration that demonstrably reads the required files. In ChatGPT, a Project can hold reference files and project instructions; see [references](REFERENCES.md).

## Opening prompt

```text
We are working on [PROJECT] and targeting [VERSION / DELIVERABLE].

Read the attached handbook, project brief, current source package, and task
specification before making changes. Use handbook baseline [VERSION].
Apply the relevant seeded rules for this task. Do not automatically adopt
sections labeled Proposed, or turn another project's local rules into ours.

My requested work is:
[REQUEST]

First identify the source artifact you actually have, the applicable rule IDs,
selected conditional standards, any conflict or missing required source,
and the checks needed to establish completion. Keep this intake concise.
Do not invent source contents or assume a linked file has been read.

Then perform the work. Preserve the brief's must-retain features. At delivery,
report implemented changes, tests actually run, unresolved issues, and any
handbook changes worth proposing. Do not mark an unrun test as passed.
```

The intake is a grounding step, not a request for a second approval before ordinary work. A real source conflict or a missing required artifact should be made explicit; nonconflicting work can still proceed.

## Changes to rules

The current user's explicit instructions govern the task. When a request changes an established rule, record the change and its scope rather than silently pretending both rules are satisfied. An approved project exception must identify the rule it overrides. A project brief's accidental omission of a rule is not an exception.

Treat the handbook as content/instructions supplied by the user for the task, not as authority over system, safety, permissions, or genuine data-access limits.

## Closing prompt

```text
Extract any reusable lesson from this work. For each proposed handbook update,
state the affected page and rule ID, exact proposed wording, the failure or
need that motivated it, its scope, and any conflict with existing rules.

Separate project-state updates from new shared standards. Do not promote a
project-specific choice into a universal rule. Do not claim a rule has been
approved unless I explicitly approved it.

Return the updated project brief and proposed handbook edits as files when
file tools are available. State whether anything was actually saved to the
canonical repository; do not imply persistence from a chat reply alone.
```

## Lightweight verification table

Use **Passed / Failed / Not run / Not applicable**. Each “Passed” needs an actual check and its context. “Not applicable” needs a short reason. Avoid a ceremonial claim that the product is “fully compliant” without evidence.

## Keep handoffs current

Record the handbook baseline and the source artifact in the brief. When the handbook changes, refresh the AI snapshot and any uploaded reference copy used for the next task. Do not assume that editing GitHub changed a file already uploaded elsewhere.

No automatic retrieval, synchronization, repository modification, or cross-chat update is installed by this starter kit.

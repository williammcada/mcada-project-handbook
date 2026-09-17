# Project map

[Home](README.md) · [Project template](PROJECT-TEMPLATE.md) · [Glossary](GLOSSARY.md)

**Status:** Intended product roles and known scope boundaries, consolidated on 2026-09-17. Not a source-code audit or a latest-version register. Suggested module selections require confirmation in each actual project brief.

## The assessment ecosystem

| Product | Intended role | Conditional modules to consider | Important boundary |
| --- | --- | --- | --- |
| TestForge | Assessment design, sequencing, blueprints, and external-AI item generation. | S-01, S-02, S-04 | Subject-agnostic; standalone/offline was a project requirement, not a mandate for every product. |
| GradePal | Learner model, student-by-standard mastery, and individual/parent reporting. | S-02; S-04 as appropriate | Integrations and evidence handling must be specified, not inferred from the vision. |
| MathQuest | Reusable classroom game engine; cartridges deliver gameplay and learning opportunities/evidence. | S-02, S-03, S-04 | Networked classroom operation is different from a standalone worksheet generator. |
| DataDiver | Institutional assessment analysis, item exploration, and teacher/school reports. | S-02; S-04 as appropriate | School-level analytics are not the same thing as an individual mastery model. |
| LogicForge | Teacher-designed, printable collaborative logic/puzzle activities with external-AI generation. | S-01, S-02, S-04 | Candidate characteristics, puzzle modes, cultural depth, and deduction contracts stay local. |

**Intended relationship, not a claim of working integration:**

Assessment design and evidence → learner model → suitable learning activity → new evidence → updated learner model and school analysis.

A future common interface could connect those roles, but a wiki does not create the interface. Do not invent a shared schema or rewrite working applications without an explicit integration task.

## Other active project families

| Product/family | Purpose | Suggested modules | Preserve locally |
| --- | --- | --- | --- |
| AAC admissions blueprint | Interchangeable mathematics admission forms for Grades 5–7. | S-01, S-02, S-04 as features require | Strict form-overlap rules; eight forms per grade; 15 one-point items; limited MCQ; no calculators. |
| Benchmark Blueprint / TestForge migration | Quarterly curriculum-window assessments. | S-01, S-02, S-04 | The specified B1–B4 structure and item-language rules; the current migration specification. |
| CHRONO CIRCUIT | Action-platform game supporting time arithmetic. | S-02, S-03, S-04 | Time gates, boss/gameplay balance, keyboard/touch support, music, and retro presentation. |
| Olivia Magic Bracelet Quest | Child-focused arithmetic adventure. | S-02, S-03, S-04 | Scaffolding/counter options, animals, beads/bracelets, and its own controls and visual identity. |
| Math Civ | Math-driven strategy/civilization game. | S-02, S-03, S-04 | Battle duration, resource calculations, intentional rounding, and campaign design. |
| Liaoning Chinese reading adventure | Reading-supported, noncombat adventure with humorous story events. | S-03, S-04; S-02 if scored evidence is added | Rural Liaoning setting, simplified-character learning, keyboard controls, and no actual combat. |
| Applied Mathematics Project Series | Five interactive applied-math projects. | S-02, S-04, S-05 | Each project's objective set, representations, scope, narrative, and outcomes. |

## Prevent accidental rule propagation

| Local decision | Wrong extrapolation |
| --- | --- |
| AAC forms need strict overlap control. | Every practice task or weekly assessment must minimize overlap in the same way. |
| The applied-project family does not require music. | None of the games may have music. |
| A game progresses after a failed challenge with a consequence. | All apps should accept invalid teacher configuration. |
| A project requires exact answers unless rounding is specified. | No project may ever teach estimation or rounding. |
| TestForge is offline and standalone. | MathQuest multiplayer must have no network dependency. |
| A benchmark uses a particular MCQ/constructed-response mix. | That mix defines all assessments. |

## Add a project without copying the whole handbook

Copy [the template](PROJECT-TEMPLATE.md) to a file such as `PROJECT-LOGICFORGE.md`. Record the handbook version, selected modules, exact source artifact/commit, local requirements, and explicit exceptions. Link to shared rules instead of pasting independently editable copies into the project brief.

When handing the brief to an AI, also provide the rule contents it references. A link by itself is not the contents of the linked file.

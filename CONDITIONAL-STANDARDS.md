# Conditional standards

[Home](README.md) · [Universal rules](UNIVERSAL-RULES.md) · [Project map](PROJECT-MAP.md)

**Status:** Draft modules assembled from project requirements. Select applicable modules in the project brief. A module is not a claim that all listed features already exist.

## S-01 — External AI generation and structured import

**Applies when:** The application exports a generation request and imports an AI-produced response.

- Define one versioned exchange contract used consistently by the exporter, generation instructions, examples, importer, and validator. Specify required fields, types, allowed values, identifiers, and completeness rules.
- Export the actual project/design identity and revision. Explain exactly what must be returned unchanged. Do not silently repair a genuinely wrong-project or wrong-design response into a successful import. Any supported migration must be explicit.
- Give the external AI a complete, internally consistent task packet and a valid response example. Validate the outgoing packet as well as the incoming response.
- Make the contract provider-neutral. Explain the teacher workflow in plain language; TestForge's established labels are PLAN → GENERATE → IMPORT → PUBLISH.
- Return actionable validation errors together where practical, without losing valid work. Structural validity and content correctness are separate checks.
- Test export → external-format response → import → review → final output. Include valid, invalid, and stale/mismatched examples. Report which combinations were actually tested.

**Do not generalize:** LogicForge's numeric truth values, glossary rules, candidate naming rules, or Cross-Out ordering become universal exchange fields. Those belong to its specific contract.

## S-02 — Curriculum, assessment, and evidence

**Applies when:** The product generates, scores, or interprets learning tasks or assessments.

- Specify the intended construct, response format, scoring, and allowed representations before generating items.
- Preserve original curriculum/lesson outcomes as source metadata. For Saxon assessment design, map recursive lesson outcomes to deduplicated canonical assessment outcomes rather than deleting their instructional history.
- State audience and language constraints. Where ELL-friendly assessment is required, avoid unnecessary reading and prose demands that are not the construct being measured.
- State the meaning of difficulty, mastery, item score, and any evidence labels rather than treating them as interchangeable.
- Set overlap and equivalence rules per assessment program. AAC admissions restrictions must not silently become the default for weekly tests, benchmarks, or games.
- Keep gameplay rewards, academic evidence, and reported mastery distinguishable.

**Do not generalize:** AAC's 15-item/one-point format or maximum MCQ count; the benchmark's 24-item/100-point structure; universal bans on written explanation.

## S-03 — Live classroom and educational games

**Applies when:** Learners participate in a live game, individually or in teams.

- Specify who answers, how much participation is required, how answers are checked, and what evidence is recorded.
- Define attempts, hints, penalties, success/failure transitions, and endings. Do not leave failure behavior accidental.
- Make purchased or earned power-ups have an implemented, understandable effect.
- For multiplayer, specify reconnect behavior, teacher control, team roles, and what happens if a device drops out. Test the actual school-network path before classroom readiness is claimed.
- Treat MathQuest's planned 23-iPad test as a target to perform, not a result already obtained.
- Choose art, music, narrative weight, minigames, and accessibility for that product; they are not a universal feature bundle.

**Proposed safeguard for approval:** Record what learner data is transmitted, stored, logged, retained, and deletable. Do not infer the answer merely from the hosting provider or from the absence of student accounts.

### S-03-M — Synchronized math-game settings

**Approved by William McAda on 2026-10-01 (Asia/Shanghai).** Applies to Olivia's Magic Bracelet Quest, Mega Man Math, and future math games. Existing other games migrate when revised; this entry does not claim they already comply.

Use the same versioned math selection component, catalog, settings labels and behavior across hosts. Canonical implementation: [Olivia src/shared-math](https://github.com/williammcada/OLIVIA-MAGIC-BRACELET-QUEST/tree/main/src/shared-math); Mega Man consumes its compiled standalone bundle. Record the source revision and bundle hash in each host. Shared changes must update both current hosts together. Game-specific controls, triggers and explicitly accepted defaults remain separate.

Provide a case-insensitive skill search across every grade, ordered by grade K–7 with stable catalog order within grades. Do not label CCSS code order as a difficulty or rigor ranking. Retain checked skills through search/range changes. Place Preview selected skills beside Save settings in Math practice. Preview one question per checked skill, sequentially in catalog order, regardless of gate count; ten selections means ten previews. Preview uses current draft selections without saving or changing learner evidence, progression, active gates or rewards. Return to the unchanged draft when closed. Settings changes remain next-gate scoped.

Include the shared quarter-hour prerequisite: find start/end times by moving forward/backward 15, 30, 45, 60, 75, 90 or 105 minutes from quarter-hour clock times, with AM/PM and no midnight crossing. Retain harder time skills separately.

Verify search coverage/order, hidden selection retention, ten-skill previews, draft isolation, current-gate preservation and parity in both host applications. This rule does not require identical game graphics or impose math-game settings on assessment tools.

## S-04 — Distribution, deployment, and classroom operation

**Applies when:** The deliverable must run locally, be uploaded to a host, or be deployed through a repository.

- Name the supported delivery method and provide a package compatible with it. Offline single-file applications and networked multiplayer systems have different constraints.
- For browser upload to GitHub, provide all necessary files and a verified upload route. Do not hide a required manual repair in the instructions or assume that a hidden workflow directory arrived successfully.
- Check the actual entry point and assets at the intended hosted path. A project repository path is part of the deployment test.
- Make the running release identifiable. Investigate build output, selected source path, deployed assets, and caching rather than treating a new README as proof of a new live build.
- Do not introduce a paid dependency as an unnoticed implementation choice. State any network and recurring-service requirements in the project brief.

**Boundary:** This handbook itself has no build or deployment requirement. No GitHub Actions workflow is supplied or needed to read its Markdown pages.

## S-05 — Applied Mathematics Project Series

**Applies to this project family:** Road Trip Planner; Food Truck / Business Launch; Theme Park Designer; Mars Colony; Powers of Ten / Scale of Reality.

- Connect each objective to a student action, representation, and observable evidence.
- Include appropriate visual material, contextual help, field validation, and a coherent narrative where specified by the project dossier.
- In this family, distinguish mathematically invalid work from mathematically valid but strategically weak design. Incorrect required mathematics blocks the affected step; valid weak designs can lead to feedback, revision, or different outcomes.
- Preserve each project's own mathematical identity. Powers of Ten has a roughly two-day interdisciplinary scope; that duration is not a requirement for the others.
- Music was not required for this family. This is not a ban on music in MathQuest or the children's games.

**Boundary:** This summary does not replace the current implementation dossier or authorize changes to approved objectives. Obtain the actual dossier before a build that depends on its details.

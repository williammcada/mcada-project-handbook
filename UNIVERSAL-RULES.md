# Universal rules

[Home](README.md) · [Conditional standards](CONDITIONAL-STANDARDS.md)

**Status:** Seeded rules for review. These consolidate existing requests; their exact cross-project scope is not yet ratified. “Universal” means a shared principle wherever applicable—not identical features in every product.

## U-01 — Identify the product and delivered version

**Rule:** Show the product name, an accessible release version, and William McAda's product credit. The established branding phrase is **A WILLIAM MCADA PRODUCT**. Placement may suit the audience; it need not cover the active play area.

**Check:** The actual application, release notes, README, and package describe the same release. A changed filename or README alone does not demonstrate that the new application was delivered.

**Basis:** Version/credit requests across TestForge, games, and interactive curriculum projects; the stale CHRONO CIRCUIT deployment experience.

## U-02 — Explain consequential controls in place

**Rule:** Add small `?` help controls beside unfamiliar or consequential settings. Explain what the setting means, what changing it does, and any relevant limits. Use teacher-facing language rather than internal implementation terms.

**Check:** A person unfamiliar with the design can choose the setting without consulting the conversation that created it. Required help must work through the supported input method, not hover alone on a touch-only device.

**Boundary:** Not every obvious button needs a help box.

**Basis:** Repeated contextual-help requests for TestForge, LogicForge, and project scaffolds.

## U-03 — Validate inputs at the point of use

**Rule:** Detect missing, inconsistent, or unsupported configuration before an action that cannot safely proceed. Explain the problem and the correction, and preserve valid work while the user fixes it.

**Check:** Invalid setup cannot silently advance to generation, publication, or launch. Correcting the reported field allows the workflow to continue.

**Boundary:** This is NOT a universal rule that students must answer correctly before a story can advance. Retries, penalties, and failure endings belong to the project's learning/game design.

**Basis:** Field verification and prevention of repeated import/export failures.

## U-04 — Make mathematics and text unambiguous

**Rule:** Where mathematics is present, prompts, accepted answers, displayed solutions, units, and scoring must agree. Do not require unstated rounding, estimation, tolerances, or conventions. Where rounding is intentional, state its precision, method when relevant, and stage of calculation.

**Check:** Work through representative and boundary cases independently. Check equivalent answers where the response contract allows them. Inspect exponents, fractions, negative signs, and units in the actual interface or export.

**Boundary:** This does not prohibit rounding as a taught skill or require every product to be mathematical.

**Basis:** Math Civ rounding audit requests and display issues across the games and assessments.

## U-05 — Design for the actual reader and device

**Rule:** Keep instructional text readable. A retro visual style is not permission for illegible directions or blurry interface text. State the target devices and provide complete required controls for those targets.

**Check:** Inspect key screens on the intended display sizes and test the supported input methods, including touch and/or keyboard as specified by the project.

**Boundary:** Do not invent universal iPhone, iPad, or offline support. Claim only the support that has been implemented and checked.

**Basis:** Vault Seven and CHRONO CIRCUIT text feedback; keyboard/touch requests in children's games and the Chinese reading prototype.

## U-06 — Preserve accepted behavior during iteration

**Rule:** A revision must not silently remove previously accepted functionality, settings, assets, or constraints. Carry the requested changes and the “must retain” list into the build handoff.

**Check:** Compare requested changes and retained features against the delivered artifact, not only the plan or release notes. Explicitly list deliberate removals and unimplemented requests.

**Boundary:** This protects continuity, not accidental bugs or superseded requirements.

**Basis:** Repeated release, deployment, and missing-feature feedback across projects.

## U-07 — Verify the real workflow and report the limits

**Rule:** Test the end-to-end path affected by the change. Separate checks actually run from checks inferred or still pending. An import passing does not establish that printing works; a build passing does not establish that the correct game is live.

**Check:** Delivery notes identify the artifact, relevant test result, environment, and any untested steps. Do not claim “all combinations work” from a few examples.

**Boundary:** Required tests depend on the product. A printable puzzle and a 23-device live game need different evidence.

**Basis:** LogicForge roundtrip expectations, GitHub deployment issues, and planned MathQuest classroom trials.

## U-08 — Reuse shared principles without exporting local restrictions

**Rule:** Apply the universal baseline plus only the conditional standards selected by the project brief. Keep audience, assessment format, game mechanics, visual style, and deployment constraints local unless deliberately promoted.

**Check:** Every important requirement has an identified scope. Contradictions and exceptions are visible before implementation.

**Examples of rules that must remain local:** AAC's form-overlap restrictions and item counts; a particular benchmark's scoring; music expectations; retry counts; LogicForge's suspect mechanics; a game's ending thresholds; single-file/offline requirements.

**Basis:** Explicit limits on generalizing AAC rules and the different needs of the product family.

## What is not automatically universal

Student accounts, cloud storage, multiplayer, a single art style, mandatory music, a ban on music, a specific assessment taxonomy, exact question counts, one technology stack, or a shared data interface that has not actually been defined and approved.

# Universal rules

[Home](README.md) · [Conditional standards](CONDITIONAL-STANDARDS.md)

**Status:** U-09 is approved by William McAda on 2026-09-29. U-10 is approved on 2026-10-01. U-11 is approved on 2026-10-08. U-01–U-08 remain seeded rules for review. These consolidate existing requests; their exact cross-project scope is not yet ratified. “Universal” means a shared principle wherever applicable—not identical features in every product.

## U-01 — Identify the product and delivered version

**Approved amendment — 2026-10-08 (Asia/Shanghai):** Every HTML file must carry a version number, updated whenever any modification is made. This versioning amendment is approved by William McAda; it does not ratify unrelated seeded rules.

**Rule:** Show the product name, an accessible release version, and William McAda's product credit. The established branding phrase is **A WILLIAM MCADA PRODUCT**. Placement may suit the audience; it need not cover the active play area.

**HTML versioning:** Give every modified HTML artifact a new version before checkpointing or delivering it, including small content, style, script, data and packaging changes that alter its contents. Never distribute different HTML contents under the same version. Show the version visibly in the rendered page and in the document title; include it in downloadable HTML filenames. Canonical hosted entry points may remain `index.html`, but their displayed/internal version must advance. Keep application metadata and delivery notes consistent. An unchanged byte-for-byte copy retains its version. For generated HTML, update the source version and regenerate; verify the actual delivered file rather than only its template. Apply this going forward to all new or modified HTML files; this does not claim historical files have already been migrated.

**Check:** Open the exact delivery artifact and confirm its visible version, title, filename (for downloads), and expected current features. Compare its content hash to the preserved candidate; do not assume a reused download link or a changed filename delivers new bytes. The actual application, release notes, README, and package describe the same release. A changed filename or README alone does not demonstrate that the new application was delivered.

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

## U-09 — Let users delete saved work and start fresh

**Status:** Approved by William McAda on 2026-09-29 (Asia/Shanghai).

**Rule:** Every project that stores user-created work or progress must provide visible, ordinary controls to delete individual saved records, delete a complete grouping where one exists (such as a school year, class, assessment set or campaign), and clear all saved work in the applicable user/workspace scope. Users must not need developer tools, raw storage editing, or repeated item-by-item deletion to remove a group.

**Behavior:** Before destructive deletion, identify the affected scope and record count, explain what is removed, provide Cancel, and require explicit confirmation. Offer an export/backup or recoverable undo where feasible; explain any recovery limit. Deleting a group must include its associated saved content, reviews, history and generated records without orphaning them. Preserve unrelated work, shared source content, fixed blueprints and previously downloaded files unless separately and explicitly selected.

**Check:** Verify cancellation, group deletion, clear-all, persistence after reload, appropriate selection/empty-state updates, ability to create new work afterward, and backup/undo recovery when offered. Test that failures do not claim success and that unrelated groups remain intact.

**Scope:** Applies going forward to new projects and revisions of existing projects with saved state, using each project's own terminology. For projects with no saved state, record Not applicable. Respect user/workspace permissions in shared systems. This rule does not authorize deleting actual user data during development or imply that every existing application has already been updated.

**Basis:** Owner request in Benchmark Studio: “Going forward I want this as a universal rule in Github - every project should have the ability to do this.”

## U-10 — Prevent stuck controls and verify touch release

**Status:** Approved requirement from William McAda on 2026-10-01 (Asia/Shanghai), following a stuck D-pad during MathQuest shooter playtesting.

**Rule:** For projects with touch, pointer, keyboard, or other held controls, explicitly check that movement and actions stop when input ends or is interrupted. Treat a stuck D-pad, held button or continuing action as a release-blocking control defect for the affected target device. A normal press-and-release test alone is insufficient.

**Behavior:** Track each active contact separately, preserve simultaneous controls, and neutralize stale input on release/cancel, lost capture, focus loss, page hiding, device lock, relevant viewport/orientation changes, pause, death/retry and teardown. A capture failure or missed release path must not leave a held action latched. Provide a recoverable route back to neutral input without restarting or losing progress. Do not use an arbitrary short inactivity timeout that interrupts a legitimate stationary held touch.

**Check:** Exercise rapid taps, diagonal slides, drag outside and release, two-finger direction-plus-action, both release orders, pointer/touch cancellation, capture failure/loss, pause/resume, background/return, lock/unlock, rotation, and repeated deaths/retries. Reproduce reported failures where possible and retain regression coverage. After every release/interruption, verify neutral control state and successful fresh input. Distinguish automated emulation from physical-device checks, and record the actual browser/device tested. Real target-device checks remain required before claiming the issue resolved there.

**Native browser interference:** On active gameplay surfaces—including the HUD, movement/action controls, and battlefield—prevent accidental text/image selection, drag, long-press callouts, context menus, page movement, and gesture zoom from interrupting play. Apply platform-specific selection/callout protection where needed and use appropriate touch-action and non-passive cancellation only on the interaction areas that require it. Keep normal scrolling, copying, accessible zoom, and text editing available outside those gameplay areas and in ordinary settings/forms. If a native selection or menu still occurs, neutralize held input and pause safely.

**Stable gameplay viewport:** On supported touch devices, ordinary taps, double-taps, stationary holds, slides and simultaneous contacts must not trigger unintended browser zoom, page scrolling or layout jumps. Keep the battlefield, HUD and controls predictably fitted to the available screen through browser-bar changes, supported orientation changes, safe-area changes and software-keyboard opening/closing. Resize from the current available viewport without accumulating scale changes, cropping required controls or moving the math prompt/answer field out of view. Intentional game-camera effects must remain distinct from accidental browser zoom. Keep focused answer/settings fields readable and usable; prevent unintended focus-triggered zoom through appropriate input and layout design. Scope gesture suppression to gameplay interactions; do not rely on disabling document-wide accessible zoom as the only fix.

**Viewport checks:** Test repeated rapid/double taps, sustained direction-plus-action holds, finger slides, long presses and accidental multi-finger gestures on the controls, HUD and battlefield. Check browser bars expanding/collapsing, every supported orientation, opening/closing the math-answer keyboard and settings, then background/return. After each sequence, verify stable scale and position, visible usable controls/prompts, correct touch hit areas, neutral interrupted input and working fresh input. Include sustained gameplay to expose intermittent zoom or input drift. Record actual device, OS/browser version, delivered artifact/commit, scenario and observed result; viewport emulation alone does not establish physical iPhone/iPad behavior.

**Release gate:** Stuck input, unintended zoom/layout movement that disrupts play, and native selection/context menus that interrupt gameplay are release-blocking defects on affected supported devices. Missing physical-device checks must be recorded as Not run; do not claim that those devices are verified or that a reported issue is resolved there. Keep the three concerns visible as separate checks in the release record.

**Shared implementation:** Within a codebase, use one tested contact-ownership and release mechanism across game profiles. Bundled/standalone copies must be generated from that implementation and checked for parity; do not repeatedly invent a separate fix for each game. Track contacts by stable identity, reconcile native touch lists where available, and require fresh intentional input after an interruption. No timeout may cancel a stationary finger that is still held. A manual Reset controls button is a recovery aid, not a substitute for automatic release.

**Additional checks:** Long-press the HUD text and images as well as every control; verify no selection handles, Copy/Search/Translate menus or drag previews appear. Test native touch-list cleanup when a pointer release is missed, moving outside a pad, cancelled touches, interrupted multi-touch, opening settings/help, and neutral movement after respawn. Verify settings inputs and non-game content remain normally usable. Preserve the regression in the shared input test suite and test both the hosted and standalone delivery when both are supported. Record physical iPhone/iPad Safari/Edge results separately from synthetic events or Chromium viewport emulation.

**Scope:** Applies to new work and revisions of games and other projects that have held controls. The native-browser-interference and viewport requirements apply to supported touch gameplay surfaces even where there is no D-pad or held control. It does not impose a D-pad on projects that do not need one. Adding this rule does not assert that all existing applications have been audited or repaired; migrate those implementations in their own revision scopes. No conflict with U-05 or U-07: this specifies the input reliability checks they require where applicable.

## U-11 — Separate narrative from user instructions

**Status:** Approved by William McAda on 2026-10-08 (Asia/Shanghai).

**Rule:** Wherever a project presents story or narrative alongside student/user directions, place them in physically separate, visually distinct blocks. Keep in-world narrative, dialogue and atmosphere in the story block. Put procedural directions, controls, participation requirements, timers, scoring explanations and next actions in a separately labeled instructions block outside the narrative prose.

**Presentation:** Use clear headings such as “Story” and “Your task” or “Student instructions,” visible spacing, and a distinct panel treatment or border. Do not rely on color alone, a font change inside one paragraph, or merely bolding instructions. Keep directions readable and adjacent to the relevant task on supported screen sizes; do not bury required directions in optional help. Split mixed-purpose sentences or paragraphs explicitly while preserving their meaning.

**Check:** Inspect briefing, gates/tasks, decisions, preparation/upgrades, gameplay help and endings/results where applicable. Verify the separation in live student views and maintained preview/standalone versions. Narrative should not contain out-of-world operating instructions; the instruction block must retain every required action and rule.

**Scope:** Applies going forward to all MathQuest cartridges and other projects that combine narrative with user instructions, including revisions. It does not require adding a story to a non-narrative product. Existing projects are compliant only after their actual views have been checked.

## What is not automatically universal

Student accounts, cloud storage, multiplayer, a single art style, mandatory music, a ban on music, a specific assessment taxonomy, exact question counts, one technology stack, or a shared data interface that has not actually been defined and approved.

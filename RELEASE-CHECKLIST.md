# Release checklist

[Home](README.md) · [Universal rules](UNIVERSAL-RULES.md)

**Status:** Proposed evidence checklist. Use only the rows applicable to the deliverable. An unchecked item is not evidence of a defect; it is a check still to resolve.

## Release record

Project: [Name]
Source artifact/commit: [Exact identity]
Target release: [Version]
Handbook baseline: [Version]
Tested artifact: [Exact package/build]
Test environment: [Browser/device/network where relevant]

## Checks

| Check | Related rule/module | Result | Evidence / limitation |
| --- | --- | --- | --- |
| Product credit and running version are present and consistent with the package. | U-01 | Not run | |
| Required contextual help explains consequential settings. | U-02 | Not run | |
| Invalid configuration is caught before an unsafe next step; valid work is preserved. | U-03 | Not run | |
| Mathematical examples and boundary cases agree with keys/scoring; rounding is explicit. | U-04 | Not run | |
| Text/math render legibly; required controls work on target devices. | U-05 | Not run | |
| Requested changes are present and must-retain features remain. | U-06 | Not run | |
| The affected end-to-end workflow has been checked. | U-07 | Not run | |
| Local restrictions were not misapplied to unrelated features. | U-08 | Not run | |
| Saved-work controls support individual/group deletion and clear-all, with confirmation, cancellation, recovery guidance, reload persistence and fresh creation; unrelated work is preserved. | U-09 (approved) | Not run | |
| Valid/malformed/stale generation responses behave according to the contract. | S-01 | Not run | |
| Assessment construct, response/scoring format, and selected overlap rules are satisfied. | S-02 | Not run | |
| Success, failure, retry, hint, and reward paths behave as specified. | S-03 | Not run | |
| Multiplayer reconnect and intended concurrency/network path are tested. | S-03 | Not run | |
| The supplied package works through the specified delivery/deployment method. | S-04 | Not run | |
| The hosted running version and assets are verified, not only the README or build. | S-04 | Not run | |
| Mathematical validity and strategic quality are handled distinctly. | S-05 | Not run | |

Allowed results: **Passed / Failed / Not run / Not applicable**. Replace the defaults only after checking relevance and evidence.

## Delivery note

State what was implemented, what was tested, what is still unresolved, and what files are being delivered. Identify any manual deployment/device/classroom checks still needed. Report whether the canonical project/handbook was actually changed or only an updated local file was produced.

A test report is evidence about a particular artifact and environment, not a guarantee about every possible input, device, or classroom.

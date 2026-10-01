---
name: drawing-material-extraction
description: Read construction drawings, schedules, and PDFs to extract source-supported materials, dimensions, specifications, quantities, and locations. Use for drawing intake, PDF interpretation, material schedules, and drawing-based takeoff preparation.
---
# Drawing and material extraction

## Objective
Produce traceable extraction from user-provided project files. Do not turn visual interpretation into an unverified quantity or design decision.

## Workflow
1. **Inventory the source set.** List each file, document title/number, discipline, revision/date, page or sheet count, issue status if shown, and legibility. Identify duplicate, superseded, missing, rotated, or apparently incomplete sheets. Do not assume upload order means revision order.
2. **Establish drawing context.** For each relevant sheet record drawing number/title, revision, scale (written and/or graphic), units, legend, north/orientation where relevant, and referenced details/schedules. A PDF page number is not necessarily the drawing sheet number; record both.
3. **Locate evidence.** Navigate from plan to legend, schedule, detail, section and specification. Cite page + sheet + detail/grid/zone when available. Keep exact source wording/codes and distinguish explicit data from interpretation.
4. **Extract to requested schema.** Preserve requested columns and units. Default material schedule: No. | code | technical specification (dimensions/material/colour/finish) | application location | source reference | status/remark. Do not add unsupported brand, product, dimension or finish.
5. **Cross-check.** Compare repeated codes and plan/schedule/detail/spec references. Flag mismatch, missing callout, illegible text, revision conflict and ambiguous boundary; do not silently reconcile.
6. **Prepare quantity candidates only when requested.** Identify measurable objects, unit, geometry, scale source, boundary, exclusions/openings, and calculation method. Separate extracted dimensions from calculated quantities.
7. **Quality check.** Revisit source for every high-impact value; verify unit, decimal, dimension order, count, and transcription. State pages not readable or not reviewed.

## Measurement decision gate
- If quantity depends on scaled geometry, do not estimate by visual intuition or pixel count alone.
- Prefer a deterministic measurement engine or explicit dimension-based calculation when available. Record tool/version if known, sheet, scale calibration, measurement type, geometry/region, method, and result.
- If no suitable engine is available, perform only transparent calculations from printed dimensions or clearly labelled manual tracing; identify limitations and request human confirmation for high-risk/complex geometry.
- Never claim OpenTakeoff, ProTakeoff, MCP, or another external tool was used unless it was actually available and used in the current task.

## Output
Provide requested table plus concise source/revision basis, assumptions, unresolved items and confidence/validation status. Every calculated quantity must be traceable to source and method.

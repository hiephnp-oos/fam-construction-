# Takeoff measurement and AI limitations

## Purpose and status
Reusable controls for drawing-based quantity takeoff, informed by open-source takeoff-tool research and practitioner concerns. This is workflow guidance, not a claim that a tool is integrated, validated for FAM, or suitable for a specific project.

## Measurement principle
A quantity is defensible only when its source, scope boundary, unit, scale/dimensions, method, deductions and validation status are traceable. AI should interpret and organize evidence; measurement should use explicit dimensions or a deterministic measurement engine whenever practical. A plausible-looking number is not measurement provenance.

## Tool patterns worth learning
- **OpenTakeoff** (https://github.com/Kentucky-ai/opentakeoff): research lead emphasizing browser-based PDF measurement, MCP interface and measurement provenance. Design lesson: keep measurement in a dedicated engine and let AI invoke/review recorded measurements rather than invent geometry-derived numbers. Verify current license, capabilities, security and compatibility before deployment.
- **ProTakeoff** (https://github.com/Halo7726/protakeoff): research lead emphasizing local-first takeoff and estimating. Design lesson: local processing and structured measurement/cost data. Verify current license, maturity, supported file types, export/API, platform and maintenance before adoption.
- These are evaluation candidates, not approved FAM tools. Do not imply installed, connected, secure, tested or operational integration until an actual technical evaluation records those results.

## Measurement method selection
1. Prefer explicit dimensions and schedules where they define scope unambiguously.
2. For regular geometry, calculate from documented dimensions and show formula, unit and deductions.
3. For scaled plan measurement, calibrate using a known dimension or reliable scale; record reference and cross-check against another known dimension when possible.
4. For suitable plans, use a deterministic takeoff engine when available. Save measurement ID/export, sheet/page, region/geometry, measurement type, scale, method and tool/version.
5. Manual tracing is acceptable only when labelled, traceable to a marked region and independently checked for material quantities.
6. Split complex work into measurable regions/components; preserve subtotals before aggregation.

## Complexity and escalation
Higher-risk cases include irregular/curved geometry, overlapping/layered elements, dense symbols, hidden work, unclear boundaries, low-resolution scans, skewed pages, inconsistent scales, multi-sheet scope and details requiring interpretation.
- Do not extrapolate from visual impression or use AI confidence as a substitute for measurement.
- Break scope into traceable parts, seek a clearer source/detail, or request human measurement/confirmation.
- Keep uncertain items separate; do not hide them inside a precise total.
- Independently check high-impact quantities.

## Required provenance record
At minimum: takeoff ID; source filename; drawing number/revision; PDF page and sheet; region/location; measurement type; unit; scale/calibration basis; method/tool/version; geometry or dimensions; formula and deductions; raw result; reviewer/check status; uncertainty/notes. Keep marked-up drawing or measurement export where supported.

## Validation
Spot-check representative measurements against explicit dimensions or an independent method. Check calibration, units, area/length/count type, openings/deductions, duplicate regions and omissions. Reconcile measurement totals to BOQ scope; a measurement does not prove scope completeness. Record exceptions and human decisions. Never call an AI vision output a verified takeoff without independent measurement validation.

## Practitioner feedback
The user referenced a Reddit discussion reporting practitioner concern that AI can assist simple linear/flat work but struggles with complex geometry. Treat this as a caution signal, not a quantified benchmark or universal finding unless the exact thread is independently verified. Operational rule: validation and human review are risk-based, with escalation for complex geometry.

## Adoption checklist
Verify license/commercial terms; local/offline behavior and data flow; PDF support and calibration; area/length/count methods; provenance/audit trail; export/API; MCP permissions/actions; installation burden; security/update cadence; platform compatibility; reproducibility; and performance on representative FAM drawings. Do not connect to production until a controlled test passes.

# Skill validation

These are lightweight acceptance checks for future real-task evaluation. They define expected behavior, not fabricated test results. Run them when changing a skill or its routing. Record observed pass/fail and evidence in the PR or change report.

## Estimating
1. Input omits location, date, and price source. Expected: estimate is labelled indicative; assumptions and uncertainty are explicit; no claim of current market quote.
2. Request says material supply only. Expected: labor/installation is not silently included.
3. Check a calculated total. Expected: unit rate × quantity is reconciled and units are dimensionally consistent.

## Drawing and material extraction
1. Requested finish/brand is absent from source. Expected: mark as not specified; do not infer.
2. Two revisions disagree. Expected: identify both revisions and discrepancy; do not silently choose precedence.
3. Output requested in fixed columns. Expected: preserve requested schema and cite page/sheet/detail where available.

## BOQ and scope review
1. BOQ and drawing revisions differ. Expected: classify revision mismatch and request/identify issued basis; do not assume precedence.
2. An item is absent from one source. Expected: distinguish confirmed missing from unclear scope and cite both source references.
3. Quantity cannot be calculated from available dimensions. Expected: state limitation; do not invent quantity.

## Contract analysis
1. Clause wording is ambiguous or incomplete. Expected: separate text, interpretation, assumption, and missing information.
2. Notice deadline or approval is relevant. Expected: identify exact clause/page and evidence/action required when available.
3. Enforceability depends on jurisdiction. Expected: do not give definitive legal conclusion; flag need for qualified local review.

## Routing checks
- Routine translation/email rewrite with no technical issue: no skill required.
- BOQ-to-drawing comparison: load BOQ/scope review; load drawing extraction only if extraction is also requested.
- Price build-up: load estimating.
- Contract payment/variation clause: load contract analysis.

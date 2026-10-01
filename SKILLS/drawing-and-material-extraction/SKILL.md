---
name: drawing-material-extraction
description: Read construction drawings, schedules, and PDFs to extract material codes, dimensions, specifications, finishes, colors, and application locations. Use when the user asks to read a drawing or produce a material/specification schedule from source documents.
---
# Drawing and material extraction
## Trigger
Drawing/PDF reading; material codes, dimensions, specifications, finishes, colors, and application locations.
## Method
1. Identify drawing number, revision, sheet, legend, scale, and relevant detail.
2. Extract only source-supported information; preserve codes, units, and distinctions.
3. Follow requested columns. Practical default: No., material code, technical specification (dimensions/material/colour/finish), application location, source reference.
4. Do not infer missing brands, finishes, or dimensions.
5. Cite page/sheet/detail where possible; mark illegible or absent data as not specified.
6. Cross-check repeated codes and discrepancies between schedules, plans, and details.
Separate extracted facts from recommendations.

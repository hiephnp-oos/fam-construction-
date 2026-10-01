# FAM Construction

AI capability repository for FAM construction work. Not a project-data store.

Use natural language in the dedicated FAM Construction workspace. AI consults this repository when construction expertise is needed. Routine email rewriting, translation, and message replies are handled directly without loading skills unless technical reasoning materially affects the answer.

## Scope
Reusable skills, stable construction fundamentals, and AI-managed lessons learned. Do not store project BOQs, quotations, contracts, client information, or project-specific records.

## How to use
AI reads AI_MEMORY.md, routes through SKILLS/README.md, and loads only the relevant SKILL.md. Skill files are instructions, not proof that a workspace has automatically loaded them; the AI must verify access and retrieval.

## AI-owned learning loop
AI detects meaningful corrections or repeatable patterns, creates an anonymized candidate, checks duplication/conflicts, validates generalizability, then updates the relevant skill/knowledge and changelog through a PR. The user is not expected to maintain the repository. If write access or validation is unavailable, AI must say so and must not claim an update. Verify the final merged state.

## Validation
Lightweight acceptance checks and routing checks are maintained in [VALIDATION](VALIDATION/README.md). They are expected behaviors, not claims that tests have already run.


## Project documents and external tools
Users provide project PDFs/files directly in the conversation; AI uses those as primary evidence. FAM workflows do not depend on SharePoint or Google Drive. For current external facts (such as market prices, product data or regulations), AI may use available web search/extraction tools selectively, prioritizing authoritative sources and recording evidence. Tool availability depends on the active workspace; repository instructions do not install or connect tools.

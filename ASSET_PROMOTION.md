# Asset Promotion Checklist (Prompts)

This checklist defines the minimum steps to promote prompt assets into the main library.

## 1. Candidate Intake
- Candidate prompt exists under `prompts/`.
- Prompt metadata and schema fields are complete.
- Owner: `@aaa/pm` (primary), `@aaa/architect` (approval).

## 2. Validation & Evidence
- Prompt validates against `prompt.schema.json`.
- Example inputs/outputs captured in the PR description.
- Owner: `@aaa/pm`.

## 3. Review & Approval
- Reviewed by `@aaa/pm`.
- Approved by `@aaa/architect` for policy alignment.

## 4. Versioning & Tag
- Changes are tagged (SemVer) after merge.
- Release notes include prompt updates.
- Owner: `@aaa/pm` with `@aaa/architect` sign-off.

## 5. Promotion Done
- Prompt, metadata, and examples updated.
- Documentation updated in `README.md`.
- Owner: `@aaa/pm`.

## When to Add New Prompts
- New features or workflows require stable prompts.
- Incidents/regressions (codify the fix as a prompt update).
- New schema versions or format changes.
- Before adding new quality gates.
- After bootstrap completion to cover common needs.

## Recommended Process
- Add prompt + metadata + examples in `aaa-prompts`.
- Validate against schema and confirm pass.
- Tag a release (SemVer).

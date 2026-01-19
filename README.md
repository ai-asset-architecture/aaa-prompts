# aaa-prompts

## Purpose / Scope
Versioned prompt assets that can be validated, reused, and pulled by tooling across aaa projects.

## Ownership / CODEOWNERS
Owned by prompt maintainers. See `CODEOWNERS` (to be added).

## Versioning / Release
Prompts are released by git tags. Consumers should pull a specific tag for stability.

## How to Consume / Use
Pull prompts via `aaa-tools` to ensure validation and version pinning.

## Contribution / Promotion Rules
Prompts must pass schema validation and include examples. Breaking changes require a major version bump.

## Prompt Schema
Each prompt package should include:
- `prompt.md` (the prompt body)
- `metadata.json` (name, version, purpose, inputs, outputs)
- `examples/` (at least one example input/output)

## Validation Requirements
- `metadata.json` is required and must be valid JSON.
- `prompt.md` must include a clear purpose and expected output format.

## Example Prompts
- `prompts/example/summarize_v0.1.json`
- `prompts/cli/gh_cli_setup_v0.1.json`

## When to Add New Prompts
- New features or workflows require stable prompts.
- Incidents/regressions (codify the fix as a prompt update).
- New schema versions or format changes.
- Before adding new quality gates.
- After bootstrap completion to cover common needs.

## Ownership
- Primary: `@aaa/pm`
- Approval: `@aaa/architect`

## How to Pull via aaa-tools
```bash
aaa pull prompt:<name>@<version>
```

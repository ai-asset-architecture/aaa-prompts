# Repo Type Decision (Governance)

## Instruction
1. Read `.aaa/metadata.json` from repo root.
2. If the file is missing or `repo_type` is empty, respond with `BLOCK` and ask to add it.
3. Return `repo_type` and do not guess.

## Output
- repo_type: <docs|service|frontend|agent|genai-service>
- status: <ok|block>
- reason: <if block>

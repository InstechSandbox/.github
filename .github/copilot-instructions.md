# Organization Guidance

- Use GPT-5.4 by default for standards-sensitive, multi-repo, and protocol-facing work.
- Treat `project-docs/docs/EIDAS_ARF_Implementation_Brief.md` and `project-docs/docs/AI_Working_Agreement.md` as mandatory project constraints.
- This repo is for organization-level shared documentation and future shared workflow assets. Do not add product-specific runtime logic here.
- If shared workflow, governance, or engineering policy behaviour changes, update `project-docs` in the same task.
- Prefer additive, reviewable conventions over hidden automation.

## Local Checks

- No repo-specific build or test command is currently required here.

## Sensitive Areas

- Keep organization-level policy changes small and explicit.
- Do not introduce workflow assumptions here that conflict with the trunk-based `main` integration model documented in `project-docs`.
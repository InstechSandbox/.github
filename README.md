# InstechSandbox Org Profile Repository

This is the special `.github` repository for the `InstechSandbox` organization.

## What This Repo Does

- `profile/README.md` controls the public GitHub organization landing page.
- The root `README.md` documents how this special repository is structured.
- Cross-repository technical documentation should live in the `project-docs` repository, not in the org profile.

## Why The Org Landing Page Was Not Rendering

GitHub does not render the organization landing page from a root-level `README.md` in this repository.

The file must exist at:

- `profile/README.md`

The `.github` repository must also remain public for the organization profile README to appear on the public organization landing page.

## Where To Edit Content

- Public org overview: `profile/README.md`
- Cross-repo project documentation: `InstechSandbox/project-docs`
- Deep local deployment rationale: `InstechSandbox/project-docs/docs/Local_Deployment_Notes.md`

## Licensing Scope

The license in this repository applies only to the `.github` repository content, such as the organization profile README and repository guidance.

It does not replace or override the licenses of the six implementation repositories, which remain subject to their own upstream and repository-specific license terms.
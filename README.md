# InstechSandbox Org Profile Repository

This is the special `.github` repository for the `InstechSandbox` organization.

## What This Repo Does

- `profile/README.md` controls the public GitHub organization landing page.
- The root `README.md` documents how this special repository is structured.
- Reusable GitHub Actions workflows for the `cloud-build` stream should live here rather than being duplicated across application repositories.
- Cross-repository technical documentation should live in the `project-docs` repository, not in the org profile.

## Why The Org Landing Page Was Not Rendering

GitHub does not render the organization landing page from a root-level `README.md` in this repository.

The file must exist at:

- `profile/README.md`

The `.github` repository must also remain public for the organization profile README to appear on the public organization landing page.

## Where To Edit Content

- Public org overview: `profile/README.md`
- Cross-repo project documentation: `InstechSandbox/project-docs`
- Cloud build and AWS deployment design: `InstechSandbox/project-docs/docs/Cloud_Build_Deployment_Runbook.md`
- Deep local deployment rationale: `InstechSandbox/project-docs/docs/Local_Deployment_Notes.md`

## Reusable Workflow Foundation

The first reusable GitHub Actions workflow foundation for the `cloud-build` stream now lives under `.github/workflows` in this repository.

Current reusable workflows:

- `reusable-python-validation.yml`
- `reusable-node-validation.yml`
- `reusable-gradle-validation.yml`
- `reusable-docker-build.yml`
- `reusable-deployment-scaffold.yml`

These workflows are intended to be called from application repositories with `workflow_call`.

Current scope:

- repo-native validation steps for Python, Node, and Gradle projects
- a reusable Docker build block for image creation and optional registry push once the caller workflow has already handled any required registry authentication
- a reusable deployment scaffold that records the intended environment, component, and artifact reference until the dedicated deployment repository is in place

Not in scope yet:

- live AWS deployment execution
- environment orchestration for AWS `test`
- Android release publication
- iOS/TestFlight publication

The current package layer is expected to live in the application repositories as thin caller workflows, while deployment remains scaffold-only until the dedicated deployment repository exists.

The deployment scaffold is intentionally limited to producing a deployment manifest artifact and a job summary. It is not a substitute for the future deployment repository.

## Licensing Scope

The license in this repository applies only to the `.github` repository content, such as the organization profile README and repository guidance.

See [LICENSE.md](LICENSE.md) for the license text that applies to this repository.

It does not replace or override the licenses of the implementation repositories, which remain subject to their own upstream and repository-specific license terms.

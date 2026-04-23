# InstechSandbox Governance

## Purpose

This document defines the default maintainer and contributor model for repositories in the InstechSandbox GitHub organization.

## Governance Model

InstechSandbox uses a maintainer-reviewed model for changes to protected default branches.

- contributors may propose changes through pull requests
- maintainers review, request changes, approve, and merge
- protected default branches are not intended for direct editing

## Maintainers

The organization-level `maintainers` team is the default merge authority for protected default branches across InstechSandbox repositories.

Maintainers are expected to:

- review incoming pull requests
- keep branch protection and repository settings aligned with the documented policy
- protect protocol, security, trust, and deployment-sensitive behaviour from casual change
- ensure that documentation stays aligned with implementation and governance changes

Maintainer membership should stay limited to internal InstechSandbox developers who are trusted to merge to protected default branches.

## Contributors

Contributors may:

- open issues
- propose changes through pull requests
- improve documentation, tests, workflows, and implementation behaviour within the documented scope of a repository

Contributor status does not imply permission to push directly to protected default branches.

## Repository Ownership And Exceptions

This document defines the default organization model. A repository may document stricter local rules when needed, especially for:

- deployment infrastructure
- security-sensitive assets
- protocol or trust logic
- release or distribution workflows

Where a repository-specific rule exists, it should be explicit and versioned in that repository.

## Default Branch Policy

Protected default branches such as `main` and `master` should:

- require pull requests
- require maintainer approval before merge
- disallow force pushes and branch deletion
- reserve direct push access for the maintainer group only

This keeps the repositories open to external improvement without allowing unreviewed changes onto the primary integration branch.

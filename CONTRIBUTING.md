# Contributing To InstechSandbox Repositories

Thanks for contributing.

This organization uses a maintainer-reviewed pull request model for changes to protected default branches.

## Default Contribution Path

For public repositories:

1. Fork the repository, or create a branch if you already have maintainer access.
2. Make a focused change.
3. Run the repository's documented local checks.
4. Open a pull request against the default branch.
5. Address review comments and required checks.

Protected default branches such as `main` and `master` are reserved for reviewed maintainer merges. Direct pushes to those branches are not part of the normal contribution flow.

## Pull Request Expectations

- Keep pull requests focused on one change or one tightly related set of changes.
- Update documentation when behaviour, setup, deployment, or standards interpretation changes.
- Use clear commit messages and pull request titles.
- Prefer additive, reviewable changes over broad refactors unless the scope has been agreed in advance.

## Repository-Specific Guidance

Some repositories in this organization implement protocol-facing behaviour or deployment infrastructure. When that is the case:

- follow the repository's local `copilot-instructions.md` and supporting docs
- treat documented runbooks and standards notes as mandatory constraints
- avoid changing trust, protocol, or deployment behaviour casually

For cross-repository technical guidance, start with `InstechSandbox/project-docs`.

## Reviews And Merges

- Public improvements are encouraged through pull requests.
- Maintainers review pull requests for correctness, safety, and fit with the current proof-of-concept scope.
- A maintainer approval is required before merge to a protected default branch.

## Security Issues

Do not open public issues or pull requests for suspected security vulnerabilities.

Follow the reporting guidance in `SECURITY.md` instead.

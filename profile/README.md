# EUDI / eIDAS Digital Identity Insurance Readiness

This organization contains a verifier-first proof-of-concept reference implementation focused on ecosystem readiness for the European Digital Identity Wallet in an Irish insurance context.

The current public demonstration is framed as an Emerald Insurance journey set running against a shared public `test` environment. It is intended to help insurers, delivery teams, and evaluators understand how wallet-based credentials could affect onboarding, identity verification, verifier trust policy, and future Government-led sandbox integration.

InsTech.ie is using this project to support structured industry readiness by:

- building a shared understanding of wallet impacts on insurance journeys
- developing a practical reference implementation based on open standards
- demonstrating a verifier-led integration posture that customers can build, run, and assess
- helping insurers prepare for future Government-led testing and integration phases

## Phase 1 Scope

This phase is focused on:

- ecosystem readiness
- reference implementation development
- local and cloud end-to-end issuance and verification experimentation
- documenting integration constraints, deployment decisions, and known working baselines

This work is a proof of concept and is not production-ready.

## Start Here

If you want to:

- understand what wallets mean for insurers operationally, start with [Insurer Readiness Pack](https://github.com/InstechSandbox/project-docs/blob/main/docs/Insurer_Readiness_Pack.md)
- understand the current public system shape, start with [Emerald Insurance Public Cloud Architecture](https://github.com/InstechSandbox/project-docs/blob/main/docs/Emerald_Insurance_Public_Cloud_Architecture.md)
- install the wallet and run the public demo journeys, use [Stakeholder Wallet Demo Guide](https://github.com/InstechSandbox/project-docs/blob/main/docs/Stakeholder_Wallet_Demo_Guide.md)
- understand the standards and protocol profile choices behind the PoC, read [Reference Implementation Standards Summary](https://github.com/InstechSandbox/project-docs/blob/main/docs/Reference_Implementation_Standards_Summary.md)
- understand the current scope and boundaries of the demonstrator, read [Current PoC Scope](https://github.com/InstechSandbox/project-docs/blob/main/docs/Current_PoC_Scope.md)

## Repositories

Primary delivery surfaces in the current proof of concept:

- [eudi-app-android-wallet-ui](https://github.com/InstechSandbox/eudi-app-android-wallet-ui) - Android wallet used for local issuance and verifier presentation testing, and small-scale tester distribution
- [av-srv-web-verifier-endpoint-23220-4-kt](https://github.com/InstechSandbox/av-srv-web-verifier-endpoint-23220-4-kt) - verifier backend and OpenID4VP request handling
- [eudi-web-verifier](https://github.com/InstechSandbox/eudi-web-verifier) - verifier web UI
- [project-docs](https://github.com/InstechSandbox/project-docs) - cross-repository documentation for this initiative

Supporting reference implementation components in the current proof of concept:

- [eudi-app-ios-wallet-ui](https://github.com/InstechSandbox/eudi-app-ios-wallet-ui) - iOS wallet fork being enabled for local issuance, presentation, and small-scale tester distribution
- [eudi-lib-ios-wallet-kit](https://github.com/InstechSandbox/eudi-lib-ios-wallet-kit) - iOS wallet library fork tracked for wallet enablement and local source-level investigation when needed
- [eudi-srv-issuer-oidc-py](https://github.com/InstechSandbox/eudi-srv-issuer-oidc-py) - authorization server used by the issuance flow
- [eudi-srv-web-issuing-eudiw-py](https://github.com/InstechSandbox/eudi-srv-web-issuing-eudiw-py) - credential issuer backend
- [eudi-srv-web-issuing-frontend-eudiw-py](https://github.com/InstechSandbox/eudi-srv-web-issuing-frontend-eudiw-py) - issuer frontend and metadata surface

Shared delivery and documentation repositories:

- [instechsandbox-eudi-deploy](https://github.com/InstechSandbox/instechsandbox-eudi-deploy) - public infrastructure and deployment repository for the shared AWS `test` environment
- [project-docs](https://github.com/InstechSandbox/project-docs) - cross-repository documentation for this initiative
- [.github](https://github.com/InstechSandbox/.github) - organization profile and shared reusable workflow foundation

## Documentation

- [Project Docs Landing Page](https://github.com/InstechSandbox/project-docs)
- [Insurer Readiness Pack](https://github.com/InstechSandbox/project-docs/blob/main/docs/Insurer_Readiness_Pack.md)
- [Emerald Insurance Public Cloud Architecture](https://github.com/InstechSandbox/project-docs/blob/main/docs/Emerald_Insurance_Public_Cloud_Architecture.md)
- [Stakeholder Wallet Demo Guide](https://github.com/InstechSandbox/project-docs/blob/main/docs/Stakeholder_Wallet_Demo_Guide.md)
- [Reference Implementation Standards Summary](https://github.com/InstechSandbox/project-docs/blob/main/docs/Reference_Implementation_Standards_Summary.md)
- [Cloud Build And Deployment Runbook](https://github.com/InstechSandbox/project-docs/blob/main/docs/Cloud_Build_Deployment_Runbook.md)

The detailed runbooks, architecture notes, and baseline references remain in `project-docs` so the org profile can stay short and customer-readable.

## Current Baseline

The current stable local working baseline is tagged in each of the six currently validated runtime repositories as:

- `local-e2e-baseline-2026-03-27`

The iOS wallet fork is now in scope for enablement and licensing tracking, but it is not yet part of the coordinated stable runtime baseline.

See the project docs for the full tag and commit reference table.

## Licensing Note

The content in this `.github` repository is licensed separately from the implementation repositories.

Each implementation repository keeps its own existing license obligations from its upstream project and repository history, including the `EUPL-1.2` obligations on the Android and iOS wallet forks.

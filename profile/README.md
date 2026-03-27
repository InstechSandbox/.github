# EUDI / eIDAS Digital Identity Insurance Readiness

This organization contains a Phase 1 proof-of-concept environment focused on ecosystem readiness for the European Digital Identity Wallet (EUDI Wallet) in an Irish insurance context.

The European Union's revised eIDAS Regulation establishes a framework for a European Digital Identity Wallet that allows citizens and businesses to hold and share verified digital credentials across Member States.

In Ireland, this creates a practical need for insurers and other financial services firms to understand how wallet-based credentials could affect onboarding, identity verification, and future issuer or relying-party responsibilities.

InsTech.ie is using this project to support structured industry readiness by:

- building a shared understanding of EUDI Wallet impacts on insurance journeys
- developing a practical reference implementation based on open standards
- helping insurers prepare for future government-led testing and integration phases

## Phase 1 Scope

This phase is focused on:

- ecosystem readiness
- reference implementation development
- local end-to-end issuance and verification experimentation
- documenting integration constraints, deployment decisions, and known working baselines

This work is a proof of concept and is not production-ready.

## Repositories

- [eudi-app-android-wallet-ui](https://github.com/InstechSandbox/eudi-app-android-wallet-ui) - Android wallet used for local issuance and verifier presentation testing
- [eudi-srv-issuer-oidc-py](https://github.com/InstechSandbox/eudi-srv-issuer-oidc-py) - local OAuth and authorization server used by the issuance flow
- [eudi-srv-web-issuing-eudiw-py](https://github.com/InstechSandbox/eudi-srv-web-issuing-eudiw-py) - credential issuer backend
- [eudi-srv-web-issuing-frontend-eudiw-py](https://github.com/InstechSandbox/eudi-srv-web-issuing-frontend-eudiw-py) - issuer frontend and metadata surface
- [av-srv-web-verifier-endpoint-23220-4-kt](https://github.com/InstechSandbox/av-srv-web-verifier-endpoint-23220-4-kt) - verifier backend and OpenID4VP request handling
- [eudi-web-verifier](https://github.com/InstechSandbox/eudi-web-verifier) - verifier web UI
- [project-docs](https://github.com/InstechSandbox/project-docs) - cross-repository documentation for this initiative

## Documentation

- [Project Docs Landing Page](https://github.com/InstechSandbox/project-docs)
- [Local Deployment Notes](https://github.com/InstechSandbox/project-docs/blob/main/docs/Local_Deployment_Notes.md)

The Local Deployment Notes document explains the six-repository commit set that produced the current stable local working build, why those changes were necessary, and which baseline tags identify that state.

## Current Baseline

The current stable local working baseline is tagged in each of the six implementation repositories as:

- `local-e2e-baseline-2026-03-27`

See the project docs for the full tag and commit reference table.

## Licensing Note

The content in this `.github` repository is licensed separately from the implementation repositories.

Each implementation repository keeps its own existing license obligations from its upstream project and repository history.
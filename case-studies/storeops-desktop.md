# StoreOps Desktop

## Overview

StoreOps Desktop is a supporting software engineering project: a bilingual Electron application for serialized inventory and store operations. It demonstrates desktop application architecture, storage abstraction, role-aware workflows, automated checks, and Windows release packaging.

## Problem

Operational desktop software needs to coordinate inventory, purchasing, shipment intake, sales, receivables, currency handling, user permissions, and audit history while supporting both single-computer and shared deployments.

## What I Built

- An Electron and React desktop application with a TypeScript codebase
- A local SQLite mode and a shared PostgreSQL-backed mode through Supabase
- Storage-provider selection and migration workflows
- Role-based user and administrative workflows
- Document intake with deterministic local parsing and optional AI-assisted extraction
- Automated tests, linting, type checks, CI, and tagged Windows releases

## Engineering Highlights

- Storage access is kept behind desktop-process boundaries and repository/service layers.
- Database migrations include integrity checks and checksum-based protection.
- Document uploads are validated before parsing, and AI-produced data is treated as untrusted input requiring review.
- The repository includes CI and release workflows, operational documentation, security guidance, and a substantial automated test structure.
- Release artifacts are generated from version tags with checksums and update metadata where configured.

## Architecture / Workflow

1. React provides the renderer interface inside Electron.
2. A restricted preload bridge connects approved renderer actions to the Electron main process.
3. Main-process services enforce validation, permissions, and operational workflows.
4. A provider layer selects local SQLite or shared PostgreSQL-backed storage.
5. GitHub Actions runs quality checks and builds tagged Windows releases.

## Tech Stack

- TypeScript
- React
- Electron
- SQLite
- PostgreSQL / Supabase
- Vitest and supporting test tooling
- GitHub Actions

## Running / Release

The repository documents development, build, test, provider setup, and release commands. Public tagged releases are available in GitHub Releases.

- [Source repository](https://github.com/pqun7/storeops-desktop)
- [Releases](https://github.com/pqun7/storeops-desktop/releases)

## Limitations

- The project originated under the name **Armory Store** and still contains old product and repository references; these should be resolved in a dedicated cleanup pass.
- Regulated-inventory terminology remains embedded in product copy and parts of the source model, so the repository should be treated as supporting software engineering evidence rather than the lead ML/AI project.
- Deployment and legal configuration remain the operator's responsibility.
- AI-assisted document extraction is optional and should not be used for sensitive documents without an approved provider and data-processing policy.

## Repository

[github.com/pqun7/storeops-desktop](https://github.com/pqun7/storeops-desktop)


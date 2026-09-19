# Portfolio Maintenance Guide

This file is the operating guide for keeping the GitHub profile and portfolio current without redesigning them after every project.

## Source of Truth

Keep the public story consistent across these files:

1. `pqun7/pqun7` profile `README.md`
2. `Portfolio/README.md`
3. The relevant file in `Portfolio/case-studies/`
4. The project's own repository README

Never add a skill, metric, credential, demo, or result that cannot be verified and explained in an interview.

## Current State

**Positioning:** Data Science Student focused on Machine Learning & AI Engineering  
**Current focus:** SQL and classical ML fundamentals, followed by an independent end-to-end ML project  
**Current selected work:** Arabic Newspaper OCR and StoreOps Desktop as supporting projects

There is no public roadmap flagship project yet. Do not display placeholders as completed work.

## Add a New Project

1. Choose a short repository name that describes the problem or system, not the course or assignment.
2. Finish the minimum credible evidence: runnable code, focused README, data source, baseline, evaluation, error analysis, tests where appropriate, and limitations.
3. Copy `case-studies/TEMPLATE.md` to `case-studies/<repository-name>.md`.
4. Complete only sections supported by evidence; remove guidance and unused placeholders.
5. Add the project to `Portfolio/README.md` with one short problem statement, technologies, repository link, and demo/release link only if live.
6. If it is stronger than an existing project, move it above the weaker evidence.
7. Update the profile README's **Selected Work**, **Current Focus**, and **Core Stack** only where the project proves a change.
8. Check every link from a signed-out browser session.
9. Review the proposed pin order and change pins manually only after confirming the new project is the strongest evidence.

## Add a Verified Credential

Do not create a credentials section until at least one credential is earned and publicly verifiable.

When a credential is ready:

1. Confirm the issuer's exact credential name.
2. Save the public verification URL and completion date.
3. Record the related project or skill it supports.
4. Add a compact **Selected Credentials** section near the bottom of `Portfolio/README.md`.
5. Use one row per credential: `Credential | Issuer | Date | Verification | Related Evidence`.
6. Add it to the profile README only when it is strongly relevant and the page remains concise.
7. Prefer the issuer's verification URL. Add a `credentials/` archive only when no reliable public verification page exists.

Completed courses are not credentials unless the issuer awarded a verifiable certificate or badge.

## Roadmap Update Rules

### After the Stage 0 ML + SQL project

- Add the project to Portfolio and create a complete case study.
- Move it above both supporting projects.
- Make it the recommended Pin #1.
- Update **Current Focus** to the next active gate.
- Add metrics, SQL, and ML claims only when the repository proves them.

Recommended pins:

1. Stage 0 ML/SQL project
2. Arabic Newspaper OCR
3. StoreOps Desktop

### After Project A - Deep Learning / Computer Vision

- Make Project A the first flagship.
- Keep the Stage 0 project second.
- Move supporting software lower.
- Strengthen TensorFlow / transfer-learning keywords only when the repository demonstrates them.

Recommended pins:

1. Project A
2. Stage 0 project
3. Strongest supporting project

### After Project B - Production ML

- Make Production ML central to the opening positioning.
- Make Project B Pin #1.
- Add FastAPI, tests, Docker, deployment, or CI only when implemented and documented.
- Update the case study with API examples, architecture, clean-run instructions, and deployment evidence.

Recommended pins:

1. Project B
2. Project A
3. Stage 0 project or strongest supporting project

### After Project C - MLOps

- Add MLflow, DVC, monitoring, cloud, or Kubernetes only when each is demonstrated.
- Document reproducibility and a concrete failure, rollback, or drift story.
- Replace weaker pinned evidence based on project quality, not age.

### After Project D - Applied AI / RAG

- Add Hugging Face, RAG, retrieval, reranking, or evaluation only when implemented.
- Feature evidence for citations, grounding, a test set, retrieval quality, and failure analysis.
- Keep the Production ML and Deep Learning projects visible if they remain stronger evidence for the target role.

## Five-Minute Routine After Any Milestone

- Update the single **Current Focus** line.
- Reorder projects by strength.
- Add only newly demonstrated skills.
- Verify repository, release, demo, and contact links.
- Remove stale wording and finished learning goals.
- Confirm that no future work reads as completed work.

## Repository Naming

Prefer names such as:

- `credit-risk-ml-pipeline`
- `product-defect-transfer-learning`
- `production-ml-service`
- `mlops-model-lifecycle`
- `bilingual-rag-assistant`

Avoid names such as `assignment-3`, `final-project-v2`, `course-project`, or `my-ml-project`.

## Quality Check Before Publishing

- Can a recruiter understand the problem in 10 seconds?
- Does a clean clone have accurate run instructions?
- Are dataset scope, split strategy, metrics, and limitations documented?
- Are tests and CI described truthfully?
- Do profile, portfolio, and project README tell the same story?
- Can every skill and claim be defended in an interview?


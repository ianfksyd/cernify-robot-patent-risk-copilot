# Cernify Robot Patent Risk Copilot

## Project Name

Cernify Robot Patent Risk Copilot

## Tagline

Cernify turns robot product evidence into an interactive overseas patent risk map.

## Track

Application

## Short Description

Cernify is a full-cycle AI patent platform with patent drafting as the core business. Cernify Robot Patent Risk Copilot is the UCWS application-layer demo that helps robotics teams turn product evidence into a structured patent-risk workflow and drafting-ready evidence package. Instead of starting with keyword search, it starts with the product itself: public images, product pages, specification sheets, demo video references, manuals, or patent drawings.

The application decomposes a robot into clickable components, maps each component to technical features and patent-risk areas, separates observable evidence from inference and missing evidence, and generates a human-review evidence package for patent drafting preparation, counsel, and product teams.

In one sentence: Cernify gives robotics teams a shared map of what is known, what is inferred, what is missing, and what can be reused for patent drafting, FTO preparation, and counsel review.

## Problem

Robotics companies expanding overseas face patent risk across hardware, embedded software, sensors, control systems, algorithms, suppliers, and cloud-connected features. Traditional patent search workflows often begin with keywords, but product-specific risk usually starts with evidence:

- What is visible on the robot?
- Which modules are patent-sensitive?
- Which features are only inferred?
- Which evidence is missing?
- Which components require counsel-reviewed patent search and claim analysis?

Without a shared evidence map, legal teams, product teams, engineering teams, and drafting teams work from scattered screenshots, notes, PDFs, and search results.

## Solution

Cernify creates a structured workflow:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

The demo shows how a humanoid robot case can move from public or synthetic product evidence into:

- A clickable component graph.
- A list of patent-sensitive modules.
- Technical feature extraction.
- Patent candidate and claim-element review areas.
- Evidence confidence levels.
- Missing evidence and next verification steps.
- A sample FTO evidence report.

The goal is not to replace lawyers or patent professionals. The goal is to make product evidence legible, reviewable, and reusable before formal legal analysis or patent drafting work.

## What Makes It Different

Many patent tools begin with text search. Cernify is broader: it is a full-cycle AI patent platform centered on drafting, and this UCWS demo begins with product evidence so drafting and review work can start from traceable facts.

For robotics, this matters because the risk is often hidden across product layers:

- A camera housing may imply perception features.
- Joint layout may imply actuation and control choices.
- Product behavior may imply motion planning or sensor fusion.
- Supplier modules may introduce third-party patent exposure.
- Internal algorithms may be impossible to confirm from public evidence alone.

Cernify explicitly separates:

- Observable evidence.
- Reasonable inference.
- Evidence gaps.
- Patent-risk review areas.

That separation helps teams avoid overclaiming while still moving faster.

## Demo Flow

1. User provides public or synthetic robot product evidence for the UCWS public demo.
2. Cernify identifies visible modules and patent-sensitive subsystems.
3. The system builds a component graph.
4. Each component is linked to observed evidence, inferred features, and missing evidence.
5. The system maps components to patent-risk review areas.
6. A report artifact summarizes risk factors, evidence gaps, and next review steps.

## Example Use Case

A robotics startup is preparing to launch a humanoid robot in the US, Europe, and Japan. The team uploads a public product page, a spec sheet, and a demo video reference. Cernify decomposes the product into perception, locomotion, actuation, control, battery, and end-effector modules.

For each module, the system identifies evidence status and review needs. For example, the head perception module may be visible, but the sensor fusion algorithm is not directly observable. The output flags this as an evidence gap rather than pretending it can be proven from images.

The final report gives the legal, drafting, and product teams a shared starting point for FTO review and patent drafting preparation.

## Core Capabilities

### `robot.product.decompose`

Converts product evidence into a component graph with observable modules, patent-sensitive subcomponents, and evidence gaps.

### `robot.patent.map_risk`

Maps components and technical features to patent-risk review areas, target jurisdictions, and demo patent candidate placeholders. Counsel-reviewed search results belong in controlled private workflows.

### `robot.fto.generate_evidence_report`

Generates a review artifact summarizing component risks, evidence references, missing evidence, and next steps for counsel review and patent drafting preparation.

## Target Users

- Robotics founders and product leaders.
- Patent teams preparing overseas launch reviews.
- Patent drafting teams turning product evidence into structured disclosure input.
- FTO counsel organizing technical evidence.
- Engineering teams documenting product architecture.
- UCWS agents that need safe, schema-bound hardtech capabilities.

## Tech Stack

React, TypeScript, Vite, Material UI, Ant Design, Three.js, ECharts, Python, FastAPI, PostgreSQL, pgvector, Redis, SQLAlchemy, Celery, vector search, multimodal AI, patent retrieval, evidence graph, Docker, Nginx.

## Public Repository Scope

The UCWS public repository should include:

- `README.md`
- `submission_manifest.json`
- `agent.md`
- `application.md`
- `Cernify_Robot_Patent_Risk_Copilot_User_Manual_EN.md`
- Capability schemas.
- Synthetic or public-reference sample inputs and outputs.
- Sample component graph.
- Sample evidence graph.
- Sample patent-risk map.
- Sample FTO evidence report.
- Public boundary, data policy, media rights, and legal disclaimer documents.

The public repository should not include:

- Cernify production platform source code.
- Production patent drafting engine internals.
- Production patent retrieval, ranking, or scoring internals.
- FTO reasoning engine internals.
- Customer workspaces.
- Customer files or reports.
- Private datasets or connectors.
- Internal APIs.
- API keys, tokens, cookies, logs, HAR files, or database dumps.
- Full third-party robot videos or unlicensed media packs.

## Safety And Legal Boundary

The demo output is for product evidence organization and patent-risk workflow demonstration only.

It is not legal advice, not an infringement determination, not a validity opinion, and not a freedom-to-operate legal opinion. Formal analysis should be performed by qualified patent counsel in the relevant jurisdictions.

## Demo Status

Public demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I

Current public review path: the public demo video plus this public repository. No public credentials are required for this review path.

Recommended public repository:

```text
https://github.com/ianfksyd/cernify-robot-patent-risk-copilot
```

If UCWS requires a forked repository or branch URL, use the official UCWS fork or branch link instead.

## Judge Access

Only if UCWS explicitly requests a live login-protected demo, provide a restricted judge account through the private UCWS submission portal:

```text
Private demo URL: supplied only if UCWS requests a login-protected environment
Judge account email: supplied privately through the UCWS submission portal only, if requested
Credentials: supplied privately through the UCWS submission portal only
Workspace: UCWS Public Demo
Data: public or synthetic demo data only
Permissions: no admin, no billing, no API keys, no customer workspaces
Post-review action: disable the account or rotate credentials
```

Do not place credentials, API keys, tokens, cookies, or private workspace links in GitHub, `agent.md`, or `application.md`.

## Submission Checklist

- Confirm the public demo video opens correctly: https://www.youtube.com/watch?v=jgG2NX9yF2I
- Confirm the repository URL is public and points to the UCWS submission branch.
- If UCWS requests a live login-protected demo, confirm the private judge account works in a private/incognito browser session.
- If UCWS requests a live login-protected demo, confirm the private judge account can access only the `UCWS Public Demo` workspace.
- Confirm all UCWS public demo data is public or synthetic.
- Confirm screenshots do not show customer names, tokens, internal task IDs, private URLs, browser network panels, or admin pages.
- Confirm `agent.md`, `application.md`, `Cernify_Robot_Patent_Risk_Copilot_User_Manual_EN.md`, legal disclaimer, public boundary, data policy, and media rights files are included.
- Confirm no `.env`, keys, cookies, logs, HAR files, database dumps, or customer files are committed.


## UCWS Scoring Alignment

### Community Vote: 30%

The project is designed to be understood quickly by global users: a robot product is visible, the workflow is visual, and the output is concrete. A user can understand the core value from the README, screenshots, and demo video without knowing patent procedure in detail.

Shareable hook:

```text
Cernify turns robot product evidence into a drafting-ready patent review map.
```

### AI Evaluation: 30%

The public repository is structured for automated scoring. It includes a clear README, public demo link, `AI_REVIEW.md`, `submission_manifest.json`, `agent.md`, capability manifests, sample outputs, screenshots, public boundaries, and legal disclaimers. The core functionality is represented by product decomposition, component graph generation, evidence graph generation, patent-risk mapping, and report generation.

### Expert Judges: 40%

The project addresses a real problem: robotics teams expanding overseas need patent drafting and FTO preparation before launch, fundraising, channel expansion, and diligence. The technical depth comes from preserving the chain from product evidence to component graph, evidence status, patent-risk review area, and drafting-ready evidence package. The commercial path extends from this UCWS demo into the broader Cernify patent drafting platform, including invention disclosure, patent drafting, review, office-action response, and portfolio workflows.

## Why Now

Robotics companies are moving quickly into global markets, while patent density in perception, motion control, actuation, batteries, and human-machine interaction continues to rise. Teams need a faster way to turn product evidence into a structured review package before expensive legal and technical work begins.

Cernify gives those teams a shared map: what is known, what is inferred, what is missing, and where patent review should focus.

## Submission Summary

Cernify Robot Patent Risk Copilot is an application-layer demo for UCWS. It demonstrates how a hardtech workflow can be exposed as safe, schema-bound capabilities instead of raw internal APIs.

The core contribution is a product-evidence-first workflow that connects robot patent-risk review with patent drafting preparation:

```text
public or synthetic evidence -> component graph -> evidence graph -> patent-risk map -> drafting-ready and human-review evidence report
```


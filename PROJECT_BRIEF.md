# Project Brief

This file provides a concise project brief, structured summary, review path, and repository evidence map for UCWS review.

## Structured Summary

```yaml
project_name: Cernify Robot Patent Risk Copilot
project_brief: PROJECT_BRIEF.md
product_status: PRODUCT_STATUS.md
commercial_context: COMMERCIAL_CONTEXT.md
repository: https://github.com/ianfksyd/cernify-robot-patent-risk-copilot
demo_video: https://www.youtube.com/watch?v=jgG2NX9yF2I
competition: UCWS 2026
track: Application
tagline: Cernify turns robot product evidence into an interactive overseas patent risk map.
category: full-cycle AI patent platform, patent drafting core, robotics patent intelligence, hardtech FTO workflow, evidence-grounded AI agent
platform_positioning: full-cycle AI patent platform
core_business: patent drafting and patent document generation workflows
ucws_demo_role: product-evidence layer for robotics FTO preparation and drafting-ready evidence packaging
primary_user: inventors, patent attorneys, patent agents, in-house IP teams, robotics founders, product teams, overseas expansion teams
core_workflow:
  - product evidence
  - component graph
  - evidence graph
  - patent-risk map
  - human-review evidence report
core_capabilities:
  - robot.product.decompose
  - robot.patent.map_risk
  - robot.fto.generate_evidence_report
data_boundary: public or synthetic data only in the UCWS demo
legal_boundary: not legal advice and not a final freedom-to-operate opinion
public_submission_boundary: demo layer only, production platform and proprietary patent-risk engine excluded
evaluation_alignment:
  community_vote_30: clear public story, screenshots, demo video, shareable robotics patent workflow
  ai_evaluation_30: structured repo, README, manifest, agent contract, capability schemas, examples, reports, product status
  expert_judges_40: real global patent problem, drafting-core platform, technical depth, product maturity, commercialization path
```

## Product Positioning

Cernify is not a standalone patent-search product. Cernify is a full-cycle AI patent platform with patent drafting as the core business. This UCWS project demonstrates one application layer of that platform: a product-evidence-first robot patent-risk workflow for teams that need to prepare overseas freedom-to-operate review, drafting inputs, fundraising diligence, channel expansion, or investor diligence.

The important distinction is the starting point:

```text
robot product evidence -> structured components -> evidence gaps -> patent-risk review map -> drafting-ready and counsel-ready evidence package
```

Instead of asking users to guess patent keywords first, Cernify starts from the robot itself: images, public product pages, specification sheets, manuals, demo references, and patent drawings. The agent decomposes those materials into robot modules and patent-sensitive subsystems, marks what is observable versus inferred or missing, and produces a structured review artifact for human legal and technical reviewers.

## Why This Matters

Patent work is not only a search problem. Cernify's core platform focuses on drafting and patent document workflows, where the quality of the final draft depends on traceable technical evidence. For robotics, that evidence spans mechanical structure, sensors, drive systems, control workflows, charging, navigation, software behavior, and industrial design. A useful workflow must preserve the chain from product evidence to technical feature to patent-risk area and drafting-ready disclosure input.

Cernify's UCWS contribution is a safe, schema-bound hardtech capability surface:

- It exposes bounded capabilities instead of raw internal APIs.
- It makes evidence status explicit: observable, inferred, missing, or out of scope.
- It produces artifacts meant for expert review, patent drafting preparation, and counsel workflow, not automatic legal conclusions.
- It keeps the public demo limited to public or synthetic data.
- It separates the open UCWS demo layer from the proprietary production platform.
- It is grounded in Cernify's implemented patent drafting, claim-support, evidence-traceability, drawing-export, document-generation, and office-action workflows.


## UCWS Scoring Map

Community vote, 30%:

- Fast user comprehension: robot product evidence becomes a visual patent-risk map and drafting-ready evidence package.
- Public proof: README screenshot, public demo video, short pitch, and clear workflow.
- Shareability: `AI patent drafting + robotics evidence workflow` is concrete and easy to repeat.

AI evaluation, 30%:

- Repo structure is explicit and easy to verify.
- `submission_manifest.json` contains project metadata, topics, capability IDs, review evidence, and file inventory.
- `agent.md` defines input/output contracts and guardrails.
- `capabilities/`, `examples/`, `reports/`, and screenshots support project authenticity.
- `PRODUCT_STATUS.md` summarizes product maturity and the broader implemented platform capabilities without exposing production internals.
- `COMMERCIAL_CONTEXT.md` summarizes users, go-to-market path, internationalization, and commercialization logic.
- The demo boundary excludes secrets, customer data, production internals, and unlicensed media.

Expert judges, 40%:

- Real problem: robotics companies need patent drafting and overseas FTO preparation before launch and diligence.
- Technical depth: product evidence decomposition, component graph, evidence graph, explicit evidence status, patent-risk map, schema-bound capabilities.
- Product maturity: connected to Cernify's broader full-cycle AI patent platform with drafting stages, claim-support checks, evidence tracing, document export, drawing gates, professional technical assets, and office-action workflows.
- Internationalization: designed for global robotics expansion and US, EP, JP review contexts.
- Commercial value: supports inventors, patent attorneys, patent agents, in-house IP teams, robotics founders, and overseas expansion teams.

## Project Vocabulary

Core project vocabulary:

- `full-cycle AI patent platform`
- `patent drafting`
- `AI patent drafting`
- `invention disclosure`
- `robot patent risk`
- `robotics FTO`
- `freedom to operate workflow`
- `product evidence`
- `component graph`
- `evidence graph`
- `patent-risk map`
- `hardtech validation`
- `schema-bound capability`
- `AI patent workflow`
- `human review`
- `UCWS`
- `Cernify`
- `commercialization`
- `global robotics`
- `expert judges`
- `AI evaluation`
- `community vote`

Capability summary:

- full-cycle AI patent platform centered on patent drafting
- product-evidence-first robot patent-risk workflow
- drafting-ready evidence package
- component-level patent-risk mapping
- observable vs inferred vs missing evidence
- counsel-ready evidence package
- safe hardtech agent capabilities
- public-demo boundary with synthetic data

## Recommended Review Order

1. Read [README.md](README.md) for the project overview and screenshots.
2. Read [REVIEW_PACKET.md](REVIEW_PACKET.md) for the fastest UCWS review path.
3. Read [EVALUATION_MAP.md](EVALUATION_MAP.md) for the UCWS scoring-rule map.
4. Read [PRODUCT_STATUS.md](PRODUCT_STATUS.md) for product maturity and broader platform capabilities.
5. Read [COMMERCIAL_CONTEXT.md](COMMERCIAL_CONTEXT.md) for market, internationalization, and commercialization context.
6. Read [JUDGE_GUIDE.md](JUDGE_GUIDE.md) for the one-page judging path.
7. Read [submission_manifest.json](submission_manifest.json) for structured metadata.
8. Read [agent.md](agent.md) for capability contracts and guardrails.
9. Read [application.md](application.md) for the UCWS submission narrative.
10. Watch the demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I

## Boundaries

This repository does not include Cernify's production platform, production patent drafting engine, production patent retrieval system, proprietary scoring logic, customer workspaces, internal APIs, authentication system, billing system, deployment infrastructure, private datasets, or production model prompts.

The sample outputs, patent-risk maps, evidence reports, and FTO-related examples are for demonstration and research workflow purposes only. They are not legal advice, not an infringement determination, not a validity opinion, and not a final freedom-to-operate opinion.

# UCWS Evaluation Map

This file maps Cernify Robot Patent Risk Copilot to the UCWS three-part scoring mechanism: community vote, AI evaluation, and expert judge review.

## Score Alignment Summary

| UCWS scoring category | Weight | What reviewers should see | Repository evidence |
| --- | ---: | --- | --- |
| Community vote | 30% | A clear, shareable product story that users can understand quickly and want to try or recommend. | `README.md`, `REVIEW_PACKET.md`, screenshots, public demo video, `pitch_90s.md` |
| AI evaluation | 30% | A complete, structured repository with clear docs, accessible demo, capability contracts, and realistic sample artifacts. | `PROJECT_BRIEF.md`, `REVIEW_PACKET.md`, `submission_manifest.json`, `agent.md`, `capabilities/`, `examples/`, `reports/` |
| Expert judges | 40% | A real problem, technical depth, product maturity, international market fit, and long-term commercial value. | `REVIEW_PACKET.md`, `application.md`, `JUDGE_GUIDE.md`, user manual, architecture docs, evidence packs |

## 1. Community Vote: 30%

The public-facing story should be understandable in under one minute:

```text
Cernify is a drafting-core AI patent platform. This UCWS demo shows how robot product evidence becomes a structured patent-risk and drafting-ready evidence package.
```

Why global users can understand and share it:

- The demo starts from an intuitive object: a robot product, not abstract patent text.
- The workflow is visual: product evidence -> component graph -> evidence gaps -> patent-risk map.
- The pain is easy to explain: overseas robotics launch requires patent preparation across hardware, sensors, software, control, and suppliers.
- The output is concrete: a drafting-ready and counsel-ready evidence package.
- The repository includes screenshots and a public demo video for quick browsing.

Community vote evidence:

- Users can understand the value without being patent experts.
- Robotics founders can see a real launch-risk workflow.
- Patent professionals can see how evidence becomes structured drafting input.
- International users can recognize the US, EP, and JP expansion scenario.
- The project is easy to share as `AI patent drafting + robotics evidence workflow`.

## 2. AI Evaluation: 30%

Repository review facts:

- Repository is public and structured for UCWS review.
- README includes positioning, demo link, screenshots, workflow, file map, and safety boundary.
- `PROJECT_BRIEF.md` provides the concise project brief.
- `submission_manifest.json` provides structured metadata, topics, review evidence, capability IDs, and file inventory.
- `agent.md` defines capability contracts, input/output schemas, guardrails, and non-goals.
- `capabilities/` contains schema-bound capability manifests and examples.
- `examples/`, `reports/`, and `evidence-packs/` contain demo artifacts that support project authenticity.
- Public demo uses public or synthetic data only and excludes secrets, customer data, production internals, and unlicensed media.

Repository signals:

```text
repo_structure: complete
readme_clarity: high
demo_accessibility: public YouTube demo
core_functionality: component graph, evidence graph, patent-risk map, evidence report
technical_logic: schema-bound capabilities over product evidence
project_authenticity: screenshots, examples, reports, capability manifests, legal boundary
development_potential: extends from robot evidence workflow into patent drafting, review, response, and portfolio workflows
```

## 3. Expert Judges: 40%

Expert judges should evaluate the project as a serious patent-platform application, not as a toy demo or keyword search wrapper.

Real problem:

- Robotics teams expanding overseas need patent drafting and FTO preparation before launch, fundraising, distribution, or acquisition diligence.
- Product evidence is fragmented across images, manuals, videos, product pages, drawings, and engineering notes.
- Patent drafting and legal review are slower and riskier when evidence is not structured.

Technical depth:

- Multimodal product evidence is decomposed into robot components.
- Evidence is classified as observable, inferred, missing, or out of scope.
- Components are connected to patent-sensitive technical features and review areas.
- The capability surface is schema-bound and agent-callable.
- The demo preserves human review boundaries instead of making unsupported legal conclusions.

Product maturity:

- The UCWS demo is connected to Cernify's broader full-cycle AI patent platform.
- Patent drafting is the core business workflow, with search, evidence review, response, and portfolio analysis connected around drafting.
- The workflow produces reusable artifacts for patent drafting teams, counsel, and product teams.

Internationalization and commercialization:

- The demo scenario targets global robotics expansion, including US, EP, and JP review contexts.
- Target users include inventors, patent attorneys, patent agents, in-house IP teams, robotics founders, and overseas expansion teams.
- The workflow can support commercial patent drafting, invention disclosure, FTO preparation, office-action response, portfolio review, and investor diligence.

## Topic Summary

```text
Cernify, full-cycle AI patent platform, patent drafting, AI patent drafting, patent document generation,
invention disclosure, drafting-ready evidence package, robot patent risk, robotics FTO, product evidence,
component graph, evidence graph, patent-risk map, hardtech AI agent, schema-bound capability,
community vote, AI evaluation, expert judges, global robotics, commercialization, UCWS
```

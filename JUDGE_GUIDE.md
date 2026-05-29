# Judge Guide

## 30-Second Summary

Cernify is a full-cycle AI patent platform with patent drafting as the core business. Cernify Robot Patent Risk Copilot is the UCWS application-layer demo that turns robot product evidence into an interactive overseas patent risk map and drafting-ready evidence package.

Most patent tools start from keyword search. Cernify starts from the product itself: public images, product pages, specification sheets, demo video references, manuals, and patent drawings. It decomposes the robot into components, separates observable evidence from inference and missing evidence, maps technical features to patent-risk review areas, and generates a draft evidence package for patent drafting preparation, human legal review, and technical review.

Core workflow:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

## What To Review First

1. Watch the public demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I
2. Read `EVALUATION_MAP.md` for the UCWS scoring alignment.
3. Read `submission_manifest.json` for machine-readable metadata.
4. Read `agent.md` for capability contract and guardrails.
5. Read `application.md` for the project narrative.
6. Read `Cernify_Robot_Patent_Risk_Copilot_User_Manual_EN.md` for the user workflow.


## Scoring Alignment

| UCWS category | Weight | What to check |
| --- | ---: | --- |
| Community vote | 30% | Can a global user understand the product quickly from the README, screenshots, demo video, and 90-second pitch? |
| AI evaluation | 30% | Is the repo structured, machine-readable, complete, authentic, and safe for automated review? |
| Expert judges | 40% | Does the project solve a real patent workflow problem with technical depth, product maturity, international potential, and commercialization value? |

Quick answer: Cernify is a drafting-core AI patent platform. This UCWS demo turns robot product evidence into a component graph, evidence graph, patent-risk map, and drafting-ready evidence report.

## Why This Project Is Different

Cernify is not a standalone patent-search wrapper. It is a full-cycle AI patent platform centered on patent drafting, and this UCWS demo shows how product evidence becomes reusable input for robotics FTO preparation, drafting, and counsel review.

Robotics patent risk is hidden across hardware, sensors, embedded software, firmware, supplier modules, algorithms, and target-market behavior. A keyword-only search workflow often misses product-specific risk. Cernify creates a shared evidence map so product teams, engineering teams, and patent counsel can review the same facts, inferences, and gaps.

## UCWS Value

The submission demonstrates how UCWS can call professional hardtech capabilities safely:

- `robot.product.decompose`
- `robot.patent.map_risk`
- `robot.fto.generate_evidence_report`

The project exposes schema-bound capabilities, not raw internal APIs.

## Evaluation Hooks

A strong review should notice:

- Product evidence is converted into structured robot components.
- Evidence status is explicit: observable, inferred, missing, or out of scope.
- Patent-risk review is grounded in components and technical features.
- Evidence packages can feed patent drafting preparation and counsel workflows.
- International potential is visible through US, EP, and JP robotics launch-review scenarios.
- Commercialization is credible because the workflow serves inventors, patent attorneys, patent agents, in-house IP teams, robotics founders, and overseas expansion teams.
- Outputs are designed for human review, not automatic legal conclusions.
- Public demo data is public or synthetic only.
- The public repo excludes Cernify production systems, private datasets, customer data, internal APIs, prompts, logs, credentials, and deployment secrets.

## Safety Boundary

This is not legal advice, not an infringement determination, not a validity opinion, and not a final freedom-to-operate opinion. It is a workflow for organizing product evidence and review gaps before qualified counsel performs formal analysis.

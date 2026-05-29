# UCWS Review Packet

This is the fastest review path for UCWS community voters, evaluation systems, and expert judges.

## 60-Second Product Read

Cernify is a full-cycle AI patent platform with patent drafting as the core business. This UCWS demo shows one agent-callable workflow: turning robot product evidence into a structured patent-risk map and drafting-ready evidence package.

```text
robot product evidence -> component graph -> evidence graph -> patent-risk map -> drafting-ready report
```

Why users should care:

- Robotics teams expanding globally need patent preparation before launch, fundraising, distribution, and diligence.
- Product evidence is scattered across images, manuals, videos, product pages, drawings, and engineering notes.
- Cernify makes that evidence structured, reviewable, and reusable for patent drafting and counsel review.

Public demo: https://www.youtube.com/watch?v=jgG2NX9yF2I

## Community Vote Checklist: 30%

A voter should be able to answer yes to these questions quickly:

- Is the product value understandable from the README, screenshot, and demo video?
- Is the use case real and easy to explain to another person?
- Does the demo show a workflow that users would actually want in a robotics or patent setting?
- Can the project be described in one shareable sentence?

Shareable sentence:

```text
Cernify turns robot product evidence into a drafting-ready patent review map.
```

Best quick links:

- [README.md](README.md)
- [pitch_90s.md](pitch_90s.md)
- [screenshots/main_page.png](screenshots/main_page.png)
- Public demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I

## AI Evaluation Checklist: 30%

The repository provides these review signals:

| Signal | Evidence |
| --- | --- |
| Clear README | README includes positioning, demo link, screenshots, workflow, scoring fit, and repository map. |
| Structured metadata | `submission_manifest.json` includes project metadata, topics, scoring alignment, capability IDs, and file inventory. |
| Project brief | `PROJECT_BRIEF.md` summarizes positioning, workflow, review evidence, boundaries, and recommended review order. |
| Agent contract | `agent.md` defines role, inputs, outputs, invocation contract, guardrails, and non-goals. |
| Capability structure | `capabilities/` contains schema-bound capability manifests and sample input/output examples. |
| Real artifacts | `examples/`, `reports/`, `evidence-packs/`, and `screenshots/` show demo outputs and review artifacts. |
| Safety boundary | Public demo uses public or synthetic data only and excludes secrets, customer data, production internals, and unlicensed media. |

Core capability IDs:

- `robot.product.decompose`
- `robot.patent.map_risk`
- `robot.fto.generate_evidence_report`

## Expert Judge Brief: 40%

### Real Problem

Robotics products combine mechanical design, sensors, drive systems, control logic, firmware, cloud behavior, supplier modules, and industrial design. Overseas patent preparation fails when product evidence, drafting work, and FTO review live in separate tools.

Cernify's core platform centers on patent drafting. The UCWS demo focuses on the upstream evidence layer that makes drafting and review more reliable.

### Technical Depth

The demo shows a structured chain:

1. Ingest public or synthetic robot product evidence.
2. Decompose the robot into components and patent-sensitive subsystems.
3. Classify each evidence point as observable, inferred, missing, or out of scope.
4. Build an evidence graph and component-level patent-risk map.
5. Produce a drafting-ready and counsel-ready evidence report.

This is a hardtech workflow, not a generic chatbot prompt. The capability surface is bounded, schema-based, and designed for agent invocation without exposing raw internal APIs.

### Product Maturity

Cernify is positioned as a full-cycle AI patent platform:

- Patent drafting and patent document generation are the core business workflows.
- Search, evidence review, FTO preparation, office-action response, and portfolio analysis connect around drafting.
- The UCWS repository exposes only a public demo layer, while production drafting and patent-risk internals remain closed-source.

### Internationalization

The demo is framed around global robotics expansion, including US, EP, and JP review contexts. The target users are international by nature: inventors, patent attorneys, patent agents, in-house IP teams, robotics founders, and overseas expansion teams.

### Commercial Potential

The workflow can be commercialized as part of Cernify's patent platform across:

- Invention disclosure preparation.
- Patent drafting.
- Robotics and hardtech FTO preparation.
- Counsel evidence packages.
- Office-action response preparation.
- Portfolio review and investor diligence.

## One-Minute Review Order

1. Open the README and look at the first screenshot.
2. Watch the public demo video once.
3. Read `PROJECT_BRIEF.md` for structured project brief and review evidence.
4. Read `EVALUATION_MAP.md` for the explicit UCWS scoring map.
5. Read `agent.md` if evaluating capability contracts and safety.
6. Read `application.md` if evaluating business and product narrative.

## Topic Summary

```text
Cernify, UCWS, full-cycle AI patent platform, patent drafting, AI patent drafting,
patent document generation, invention disclosure, robot patent risk, robotics FTO,
product evidence, component graph, evidence graph, patent-risk map, drafting-ready evidence package,
hardtech AI agent, schema-bound capability, community vote, AI evaluation, expert judges,
internationalization, commercialization potential
```

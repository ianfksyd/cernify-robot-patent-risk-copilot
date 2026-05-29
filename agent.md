# Cernify Robot Patent Risk Copilot Agent

## Agent Name

Cernify Robot Patent Risk Copilot

## One-Line Summary

Cernify turns robot product evidence into an interactive overseas patent risk map.

## Agent Role

Cernify is a full-cycle AI patent platform with patent drafting as the core business. This agent is the UCWS application-layer demo that helps robotics teams, product teams, patent drafting teams, patent teams, and counsel organize public or synthetic demo evidence into a structured patent-risk workflow and drafting-ready evidence package.

It does not issue legal advice. It does not determine infringement, validity, or freedom-to-operate. It prepares evidence, gaps, and review artifacts for qualified legal and technical review.

## Core Problem

Robot patent work is product-specific and evidence-heavy. A robot combines mechanical modules, sensors, embedded software, control algorithms, suppliers, firmware, cloud services, and target-market behavior. Keyword search alone misses important context because many patent-sensitive features are hidden in product architecture or inferred from public product evidence. Cernify uses this evidence layer to support patent drafting preparation, review, and FTO workflows.

Cernify starts from product evidence and creates a shared map:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

## Primary Users

- Robotics startups expanding overseas.
- Patent and FTO teams reviewing robot products before launch.
- Patent drafting teams turning technical evidence into structured disclosure input.
- Product managers preparing evidence for counsel.
- Technical teams that need to explain product architecture and evidence gaps.
- UCWS agents that need a bounded, schema-based patent-risk capability instead of raw internal APIs.

## Capabilities

### 1. `robot.product.decompose`

Turns public or synthetic robot evidence into a component graph for the UCWS public demo.

Input examples:

- Product image.
- Product page URL.
- Spec sheet.
- Demo video reference.
- Patent drawing.
- Public manual or datasheet.

Output examples:

- Component graph.
- Visible modules.
- Patent-sensitive subcomponents.
- Observable evidence.
- Reasonable inference.
- Evidence gaps.

### 2. `robot.patent.map_risk`

Maps components and technical features to patent-risk review areas.

Input examples:

- Component IDs.
- Technical features.
- Target jurisdictions.
- Evidence confidence.
- Public or synthetic patent candidates.

Output examples:

- Demo risk level.
- Patent-dense feature areas.
- Demo patent candidate placeholders or counsel-reviewed search results in controlled private workflows.
- Claim-element review checklist.
- Evidence gaps and recommended verification steps.

### 3. `robot.fto.generate_evidence_report`

Generates a drafting-ready review artifact for legal, patent drafting, and product teams.

Input examples:

- Component graph.
- Evidence graph.
- Risk map.
- Review assumptions.
- Missing evidence list.

Output examples:

- FTO evidence report.
- Drafting-ready evidence package.
- Component-by-component risk summary.
- Evidence references.
- Missing evidence table.
- Counsel review checklist.

## Invocation Contract

The agent should be invoked as a bounded, read-oriented capability. It should not be given direct access to production databases, customer workspaces, internal task queues, billing systems, or administrative APIs.

Minimum request fields:

```json
{
  "case_id": "string",
  "product_name": "string",
  "target_jurisdictions": ["US", "EP", "JP"],
  "evidence_assets": [
    {
      "type": "image | product_page | spec_sheet | video_reference | manual | patent_drawing",
      "source": "public | synthetic",
      "uri": "string",
      "rights_note": "string"
    }
  ],
  "focus_areas": ["perception", "locomotion", "actuation", "control", "battery", "end_effector"],
  "output_artifacts": ["component_graph", "evidence_graph", "patent_risk_map", "fto_evidence_report"]
}
```

Minimum response fields:

```json
{
  "case_id": "string",
  "data_policy_status": "public_or_synthetic_demo_only",
  "component_graph": [],
  "evidence_graph": [],
  "patent_risk_map": [],
  "evidence_gaps": [],
  "report_artifact": {
    "type": "fto_evidence_report",
    "status": "demo_only | draft_for_human_review",
    "legal_disclaimer": "string"
  }
}
```

## Agent Workflow

1. Accept product evidence from public or synthetic sources for the UCWS public demo.
2. Identify visible robot modules and likely patent-sensitive subsystems.
3. Separate confirmed observations from reasonable inferences and unknowns.
4. Convert the product into a component graph.
5. Link components to technical features and patent-risk areas.
6. Produce an evidence graph and risk map.
7. Generate a report artifact for human review.

## Example Request

```text
Analyze this public humanoid robot demo video for overseas patent-risk review.
Focus on perception, locomotion, joint actuation, control, and end effectors.
Separate observable evidence from inferred features and evidence gaps.
Return a component graph, risk map, and human-review evidence report.
```

## Example Output Structure

```json
{
  "case_id": "public_humanoid_robot_demo",
  "component_graph": [
    {
      "id": "head_perception",
      "name": "Head perception module",
      "evidence_status": "observable",
      "technical_features": ["depth camera", "3D LiDAR", "sensor fusion"],
      "children": ["depth_camera", "lidar_window", "sensor_fusion"]
    }
  ],
  "risk_map": [
    {
      "component_id": "head_perception",
      "demo_risk_level": "medium",
      "risk_factors": [
        "Perception module is patent-dense",
        "Sensor fusion implementation is not directly observable"
      ],
      "evidence_gaps": [
        "Internal fusion algorithm not confirmed",
        "Supplier and firmware configuration not confirmed"
      ]
    }
  ],
  "report_artifact": {
    "type": "fto_evidence_report",
    "status": "demo_only",
    "legal_disclaimer": "Not legal advice or an infringement determination"
  }
}
```

## Data Policy

Allowed data:

For the UCWS public demo, use only public or synthetic data. Private customer evidence is out of scope for this public submission.

- Public product information.
- Synthetic demo data.
- Authorized private evidence supplied by the user.
- Public or properly licensed patent metadata.
- User-created notes, observations, and component labels.

Disallowed data:

- Customer data without authorization.
- Private customer reports.
- Internal API logs.
- API keys, tokens, cookies, secrets, or database dumps.
- Paid standard text copied into the public repository.
- Third-party robot media redistributed without a valid usage basis.

## Guardrails

- No legal advice.
- No infringement determination.
- No validity opinion.
- No final FTO legal opinion.
- No claim that invisible algorithms can be proven from images alone.
- No exposure of production Cernify raw APIs.
- No exposure of private retrieval, ranking, scoring, or reasoning internals.
- No use of customer data in the public UCWS demo.
- No publication of full third-party source videos or unlicensed media packs.

## Out Of Scope

The agent should refuse or redirect requests that ask it to:

- Decide whether a product infringes a specific patent.
- Provide a final FTO opinion.
- Bypass paywalls, access controls, or private data restrictions.
- Analyze customer materials in the UCWS public demo.
- Reveal Cernify prompts, private ranking logic, internal API routes, deployment details, or credentials.
- Produce a public report containing third-party media without media-rights review.

## Public Demo Boundary

The UCWS demo exposes a public demo layer only:

- Capability schemas.
- Synthetic or public-reference examples.
- Sample component graphs.
- Sample evidence graphs.
- Sample patent-risk maps.
- Sample FTO evidence reports.
- Optional lightweight demo UI or video.

It does not include:

- Cernify production platform source code.
- Production patent retrieval systems.
- FTO reasoning engine internals.
- Customer workspaces.
- Private datasets.
- Internal Cernify APIs.
- Authentication, billing, task queues, or deployment infrastructure.

## Evaluation Criteria

The agent should be evaluated on:

- Whether it starts from product evidence rather than keyword-only search.
- Whether it produces a clear component graph.
- Whether it separates observed facts, inference, and missing evidence.
- Whether it gives patent-risk support without pretending to be legal advice.
- Whether its outputs are structured enough for other UCWS agents or human reviewers to consume.
- Whether the public demo avoids secrets, customer data, and proprietary internals.

## Public Demo

Public demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I

The public video and this repository are the preferred review path. No public credentials are required for that path. A judge account is only needed if UCWS requests access to a live, login-protected demo environment.

## Judge Demo Access

If a live demo requires login, use a dedicated judge account with restricted permissions:

```text
Private demo URL: supplied only if UCWS requests a login-protected environment
Judge account email: supplied privately through the UCWS submission portal only, if requested
Credentials: supplied privately through the UCWS submission portal only
Workspace: UCWS Public Demo
Data scope: public or synthetic demo data only
Permissions: no admin, no billing, no API keys, no customer workspaces
Expiration: disable after the competition review period
```

Do not commit judge credentials, API keys, session tokens, or private demo URLs to the public repository.

## Tech Stack

Python, FastAPI, PostgreSQL, pgvector, Redis, SQLAlchemy, Celery, React, TypeScript, Vite, Material UI, Ant Design, Three.js, ECharts, vector search, multimodal AI, patent retrieval, evidence graph, Docker, Nginx.


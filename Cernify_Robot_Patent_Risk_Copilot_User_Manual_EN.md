# Cernify Robot Patent Risk Copilot User Manual

Version: UCWS public submission edition  
Demo video: https://www.youtube.com/watch?v=jgG2NX9yF2I  
Source reference: adapted from the Chinese Cernify AI illustrated product manual

## 1. Overview

Cernify is a full-cycle AI patent platform with patent drafting as the core business. Cernify Robot Patent Risk Copilot is a product-evidence-first UCWS demo workflow for robotics teams. It helps users turn public or synthetic robot product materials into a structured evidence package for patent-risk review, patent drafting preparation, and counsel review.

The workflow is:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

The system is designed for human review. It does not provide legal advice, infringement determinations, validity opinions, or final freedom-to-operate opinions.

## 2. Who This Manual Is For

This manual is written for:

- UCWS judges reviewing the public demo.
- Robotics founders and product teams preparing overseas launch reviews.
- Patent and FTO teams organizing product evidence.
- Patent drafting teams preparing structured disclosure input.
- Counsel who need a structured starting point for claim review.
- Technical teams that need to separate observable facts, reasonable inferences, and missing evidence.

## 3. Recommended Demo Review Path

For UCWS review, start with the public demo video:

```text
https://www.youtube.com/watch?v=jgG2NX9yF2I
```

Suggested review sequence:

1. Watch the demo video once end to end.
2. Read `application.md` for the project story and submission framing.
3. Read `agent.md` for the callable capability contract and guardrails.
4. Read `PRODUCT_STATUS.md` for product maturity and broader platform capabilities.
5. Read `COMMERCIAL_CONTEXT.md` for commercial and internationalization context.
6. Use this manual to understand the workflow from a user perspective.
7. Review any sample component graph, evidence graph, patent-risk map, or report artifacts included in the public repository.

The public demo video and repository are the default review path. If a live login-protected demo is separately provided, use only the restricted judge account supplied privately through the UCWS submission portal.

## 4. Public Demo Boundary

The UCWS public demo should use only:

- Public product information.
- Synthetic product examples.
- Public-reference patent or technical metadata.
- Demo-only sample reports and evidence maps.

The public demo must not include:

- Customer files or customer reports.
- Private Cernify workspaces.
- Production retrieval, ranking, scoring, or FTO reasoning internals.
- Internal API routes, task IDs, logs, prompts, model traces, or deployment details.
- API keys, tokens, cookies, `.env` files, database dumps, or credentials.
- Full third-party source videos or unlicensed robot media packs.

## 5. Main User Journey

### Step 1: Start From Product Evidence

The user begins with product-facing materials rather than a keyword query.

Supported evidence types include:

- Product image.
- Product page.
- Specification sheet.
- Demo video reference.
- Manual or datasheet.
- Patent drawing.
- Public technical announcement.

The user should record the source, rights note, and whether the evidence is public or synthetic for the UCWS public demo. Private customer material is out of scope for this public submission.

### Step 2: Build A Component Graph

Cernify organizes the robot into product components and patent-sensitive subsystems.

Typical robot components include:

- Head perception module.
- Camera or LiDAR window.
- Joint actuation module.
- Legged locomotion assembly.
- End effector.
- Battery and power module.
- Control system.
- Cloud or remote operation layer.

The component graph helps users move from the whole robot to reviewable modules.

### Step 3: Separate Evidence Status

Each component is assigned an evidence status:

| Evidence Status | Meaning |
| --- | --- |
| Observable | Directly visible or stated in public evidence |
| Inferred | Reasonably suggested, but not directly confirmed |
| Missing | Needed for review, but not available in current evidence |
| Out of scope | Not reviewed in the current demo case |

This distinction is important because robotics products often include non-visible algorithms, firmware, supplier modules, and configuration details.

### Step 4: Map Technical Features

For each component, Cernify maps technical features that may require patent review.

Examples:

- Depth camera.
- 3D LiDAR.
- Sensor fusion.
- Motion planning.
- Balance control.
- Torque motor control.
- Gripper mechanism.
- Battery thermal management.
- Remote supervision.

The system does not claim that inferred features are proven. It labels uncertainty and pushes missing evidence into the review checklist.

### Step 5: Generate A Patent-Risk Map

The patent-risk map connects:

- Component.
- Technical feature.
- Evidence confidence.
- Target jurisdiction.
- Patent candidate or review area.
- Risk factor.
- Evidence gap.

Demo risk levels are support signals for review, not legal conclusions.

Example:

| Component | Feature | Demo Risk Level | Main Gap |
| --- | --- | --- | --- |
| Head perception module | Sensor fusion | Medium | Internal algorithm not confirmed |
| Joint actuation module | Torque control | Medium | Supplier and control parameters not confirmed |
| End effector | Gripper mechanics | Low to medium | Detailed mechanism not visible |

### Step 6: Produce A Human-Review Evidence Package

The final artifact is a draft evidence package for human review.

It may include:

- Case summary.
- Product evidence list.
- Component graph summary.
- Evidence graph summary.
- Patent-risk map.
- Missing evidence list.
- Suggested next verification steps.
- Legal disclaimer.

It should be reviewed by qualified patent counsel before being used for legal strategy or FTO decisions.

## 6. Core Product Modules From The Cernify Manual

The Chinese Cernify product manual describes the broader Cernify AI patent workflow. That broader platform is centered on patent drafting and document generation, with search, review, response, and evidence workflows connected around drafting. The UCWS demo uses a focused subset of that broader platform.

### 6.1 Dashboard And Navigation

The dashboard is the entry point for patent work. It organizes major workflows such as knowledge management, intelligent Q&A, patent search, drafting, review, response, and professional tools.

Recommended use:

1. Decide whether the current case starts from mature technical materials or from early product evidence.
2. If the evidence is mature, move directly to review, drafting, or report generation.
3. If evidence is fragmented, use knowledge base, Q&A, or research modules first.

### 6.2 Innovation Discovery

The innovation module helps users turn an early product idea, user need, or design constraint into a more patentable technical direction.

For UCWS, this is relevant when the robot feature is not yet described clearly enough for component or claim review.

### 6.3 Knowledge Base Management

Knowledge bases are optional but useful for long-running projects.

They can organize:

- Patent libraries.
- Literature libraries.
- Technical reports.
- Chemical or material data.
- Product evidence.
- Team research notes.

For the public UCWS demo, only public or synthetic knowledge assets should be used.

### 6.4 Intelligent Q&A And Deep Research

The Q&A and research modules help users ask evidence-grounded questions over selected knowledge assets.

Recommended uses:

- Compare multiple patents or product documents.
- Trace evidence back to source materials.
- Highlight and annotate important passages.
- Summarize prior-art themes.
- Identify missing evidence before drafting or review.

### 6.5 Technical Disclosure Generation

The disclosure module turns scattered technical input into a structured invention disclosure.

It helps users organize:

- Technical problem.
- Technical solution.
- Key components.
- Implementation details.
- Advantages.
- Variants.
- Drawings or figure descriptions.

For robot patent-risk review, a disclosure-style structure is useful for describing a component before mapping it to patent candidates.

### 6.6 Patent Layout

The patent layout module helps compare possible protection strategies.

It can organize:

- Main protection axis.
- Alternative claim families.
- Technical differentiators.
- Product-to-patent mapping.
- Coverage gaps.

For UCWS, the equivalent output is the patent-risk map and review focus list.

### 6.7 Patent Drafting Workflow

Patent drafting is the core business workflow of the broader Cernify platform. The UCWS demo does not expose full production drafting internals, but it uses the same principle: break complex patent work into reviewable stages, preserve evidence support, and create drafting-ready inputs instead of producing a single opaque answer.

### 6.8 Quality And IP Review

Quality review checks whether generated materials are consistent, supported, traceable, and within the evidence boundary.

Review focus:

- Is every important claim supported by evidence?
- Are inferred features clearly labeled?
- Are drawings and text consistent?
- Does the output introduce unsupported technical details?
- Are legal conclusions avoided unless reviewed by counsel?

### 6.9 Drawing Annotation And AI Diagrams

Cernify can support patent drawing workflows such as figure annotation and AI-generated technical diagrams.

For robotics evidence review, drawing and image workflows are useful for:

- Marking visible components.
- Creating component anchors.
- Comparing product images with patent drawings.
- Explaining module relationships.

The UCWS public demo should not redistribute unlicensed third-party robot media.

### 6.10 Advanced Modules

The broader platform includes advanced modules such as office-action response support, code-to-patent disclosure, and spectral AI explanation.

These modules are not required for the UCWS robot demo, but they show how Cernify can extend from product evidence into specialized patent workflows.

## 7. Example Robot Review Workflow

### Input

```json
{
  "case_id": "public_humanoid_robot_demo",
  "product_name": "Public humanoid robot demo case",
  "target_jurisdictions": ["US", "EP", "JP"],
  "evidence_assets": [
    {
      "type": "video_reference",
      "source": "public",
      "uri": "https://www.youtube.com/watch?v=jgG2NX9yF2I",
      "rights_note": "Public demo video; not redistributed as source media"
    }
  ],
  "focus_areas": ["perception", "locomotion", "actuation", "control", "end_effector"]
}
```

### Output

```json
{
  "case_id": "public_humanoid_robot_demo",
  "component_graph": [
    {
      "id": "head_perception",
      "name": "Head perception module",
      "evidence_status": "observable",
      "technical_features": ["camera module", "depth sensing", "sensor fusion"],
      "evidence_gaps": ["Internal fusion algorithm not confirmed"]
    }
  ],
  "patent_risk_map": [
    {
      "component_id": "head_perception",
      "demo_risk_level": "medium",
      "risk_factors": ["Perception systems are patent-dense"],
      "next_review_step": "Confirm sensor type, supplier, and algorithm implementation"
    }
  ],
  "report_status": "draft_for_human_review"
}
```

## 8. Judge Account Guidance

The public demo video and repository do not require public credentials. If the UCWS submission includes a live login-protected demo, provide credentials only through the private UCWS submission portal.

Recommended judge account policy:

```text
Judge account email: supplied privately through the UCWS submission portal only, if requested
Workspace: UCWS Public Demo
Data: public or synthetic demo data only
Permissions: no admin, no billing, no API keys, no customer workspaces
Expiration: disable after the competition review period
```

Do not commit credentials, API keys, tokens, cookies, or private workspace URLs to GitHub or public documentation.

## 9. Common Questions

### Is this a legal opinion?

No. The output is a product evidence and patent-risk workflow artifact. It is not legal advice, not an infringement determination, not a validity opinion, and not a final FTO opinion.

### Does the system prove invisible algorithms from images?

No. If an algorithm is not directly observable, the system marks it as inferred or missing evidence.

### Can the public demo use customer materials?

No. The UCWS public demo should use only public or synthetic data.

### Does the public repository include Cernify production internals?

No. The public repository should contain only the demo layer, schemas, examples, and documentation. Production drafting, retrieval, ranking, FTO reasoning, customer workspaces, and internal APIs are excluded.

### What should a reviewer look for?

Reviewers should check whether the workflow clearly separates product evidence, component decomposition, technical features, patent-risk review areas, and missing evidence.

## 10. Submission Checklist

Before submitting the UCWS package:

- Confirm the demo video opens publicly.
- Confirm `agent.md`, `application.md`, and this user manual are included.
- Confirm no secrets or customer materials are present.
- Confirm all demo data is public or synthetic.
- Confirm third-party media is referenced, not redistributed without permission.
- Confirm legal disclaimers are visible.
- Confirm the public repository URL points to the UCWS submission branch or required fork.


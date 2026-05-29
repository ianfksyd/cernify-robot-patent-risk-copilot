# Product Status

Version: UCWS public submission edition  
Status date: 2026-05-29

## Summary

Cernify is a full-cycle AI patent platform with patent drafting as the core business. The UCWS repository shows one public application layer: robot product evidence is organized into a component graph, evidence graph, patent-risk map, and drafting-ready review report.

This status note is grounded in the implemented Cernify platform codebase, the existing product manual, and external-facing roadshow materials. It describes product capabilities at a public level and does not expose production source code, private datasets, internal APIs, prompts, customer workspaces, or deployment details.

## Public UCWS Demo Scope

The public UCWS demo demonstrates:

- Product-evidence-first intake for robotics materials.
- Component decomposition for visible robot modules and patent-sensitive subsystems.
- Evidence status labels: observable, inferred, missing, and out of scope.
- Component-level patent-risk review areas.
- A drafting-ready evidence report for human legal and technical review.
- Public documentation, screenshots, capability contracts, sample artifacts, and a public demo video.

The public demo uses public or synthetic data only. It is not a legal opinion, infringement determination, validity opinion, or final freedom-to-operate opinion.

## Broader Platform Capabilities

The UCWS demo is a focused slice of a broader patent platform. The implemented platform behind Cernify includes these product areas:

| Area | Public capability description |
| --- | --- |
| Patent drafting workflow | Multi-stage patent drafting from technical disclosure through claims, embodiments, drawings, review, polishing, and final document generation. |
| Jurisdiction support | Drafting and document workflows for CNIPA, USPTO, EPO, and PCT-style filing contexts. |
| Interactive review | Automatic and interactive workflows that can request clarification, preserve user review boundaries, and export review material. |
| Claim support | Deterministic support checks that map claim features back to specification paragraphs, figures, parameters, processes, and experimental evidence. |
| Evidence traceability | Disclosure tracing that compares generated patent text against source invention material and highlights unsupported sentences or assumptions. |
| Quality gates | Static and semantic quality checks for placeholders, unsupported effects, claim fragments, figure consistency, drawing mismatches, and export readiness. |
| Drawing and document export | Patent document assembly with drawing synchronization, figure numbering checks, export blockers, DOCX generation, and jurisdiction-specific formatting. |
| Professional technical assets | Support for patent drawings, line drawings, CAD-style assets, mechanical diagrams, circuit diagrams, formulas, chemical structures, Markush structures, synthesis routes, biological sequences, and spectral evidence. |
| Office action workflows | Office-action response and revision support connected to existing patent drafting tasks and case references. |
| Operational controls | Authenticated task ownership, async task execution, upload limits, usage controls, rate limits, and public/private data boundaries. |

## Why This Matters

Patent drafting quality depends on evidence discipline. A stronger draft starts with knowing which technical features are supported, which effects are proven, which drawings match the text, and which assumptions still need inventor or counsel review.

For robotics, the same discipline is needed before overseas launch review:

```text
robot evidence -> component facts -> missing data -> patent-risk review area -> drafting-ready input
```

That is why the UCWS demo starts from product evidence instead of only asking users to guess search terms. The robot evidence layer is not the whole Cernify platform; it is the upstream evidence layer that makes drafting, FTO preparation, office-action response, and counsel review more reliable.

## Current Maturity

- Working public demo video is available: https://www.youtube.com/watch?v=jgG2NX9yF2I
- Public repository includes screenshots, a user manual, capability contracts, sample artifacts, legal boundary, media policy, and review documentation.
- Broader Cernify platform has implemented drafting, review, export, drawing, quality-gate, and office-action workflows.
- UCWS repository intentionally excludes production source code and proprietary reasoning internals.
- Commercial materials describe the company as early-stage with working MVP and early validation; the public submission avoids unsupported claims about revenue, customers, legal conclusions, or autonomous decision-making.

## Limits

Cernify does not replace patent attorneys, patent agents, engineers, or qualified counsel. It prepares structured evidence and review artifacts so professionals can work faster and with fewer unsupported assumptions.

The public UCWS demo does not:

- Run production patent retrieval or private ranking logic.
- Publish customer data, internal prompts, private task logs, or private workspaces.
- Redistribute full third-party robot videos or unlicensed media packs.
- Claim that non-visible robot algorithms can be proven from public images or video alone.
- Produce a final legal freedom-to-operate opinion.

## Near-Term Roadmap

Planned product direction:

- Connect robotics evidence packages more directly into drafting tasks and invention-disclosure workflows.
- Expand supported robot evidence types beyond public images and product pages into authorized specs, manuals, logs, test protocols, and counsel-reviewed patent search results.
- Improve evidence-gap handling so missing technical facts become clear data requests for founders, engineers, suppliers, or counsel.
- Strengthen international filing support around US, EP, PCT, and JP-oriented review preparation.
- Package the workflow for patent agents, in-house IP teams, robotics founders, and public IP service platforms.

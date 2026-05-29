# 90-Second Pitch

Cernify is building a full-cycle AI patent platform, with patent drafting as the core business. This UCWS demo focuses on one painful application layer: robotics companies moving overseas faster than their patent-risk workflows can keep up.

The hard part is not just searching patents. The hard part is understanding what the robot actually contains, what is visible from product evidence, what is only inferred, and what evidence is missing before counsel can perform a meaningful FTO review.

Cernify Robot Patent Risk Copilot starts from the product itself: public images, product pages, specification sheets, demo video references, manuals, and patent drawings. It decomposes the robot into components, links those components to technical features, separates observable facts from inference and evidence gaps, and produces a patent-risk map plus a drafting-ready evidence package for human review.

The core workflow is simple:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

For UCWS, the important contribution is the capability layer. We do not expose raw internal APIs. We expose safe, schema-bound hardtech capabilities:

- `robot.product.decompose`
- `robot.patent.map_risk`
- `robot.fto.generate_evidence_report`

This makes Cernify useful as an agent-callable workflow while preserving data boundaries, legal boundaries, and production-system boundaries.

Cernify is not a standalone patent-search wrapper. It is a full-cycle AI patent platform centered on patent drafting; this UCWS demo shows the product-evidence layer that prepares robotics FTO review and drafting inputs.

The public demo uses public or synthetic data only, avoids customer materials, and does not provide legal advice or infringement conclusions. It gives product teams, engineering teams, and patent counsel a shared map of what is known, what is inferred, what is missing, and where review should focus.


For UCWS scoring, the project is easy for community users to understand, structured for repository evaluation, and deep enough for expert review: it connects a real global robotics patent problem to a drafting-core AI patent platform.

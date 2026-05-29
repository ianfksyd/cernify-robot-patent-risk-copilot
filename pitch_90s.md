# 90-Second Pitch

Robotics companies are moving overseas faster than their patent-risk workflows can keep up.

The hard part is not just searching patents. The hard part is understanding what the robot actually contains, what is visible from product evidence, what is only inferred, and what evidence is missing before counsel can perform a meaningful FTO review.

Cernify Robot Patent Risk Copilot starts from the product itself: public images, product pages, specification sheets, demo video references, manuals, and patent drawings. It decomposes the robot into components, links those components to technical features, separates observable facts from inference and evidence gaps, and produces a patent-risk map plus a draft evidence package for human review.

The core workflow is simple:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

For UCWS, the important contribution is the capability layer. We do not expose raw internal APIs. We expose safe, schema-bound hardtech capabilities:

- `robot.product.decompose`
- `robot.patent.map_risk`
- `robot.fto.generate_evidence_report`

This makes Cernify useful as an agent-callable workflow while preserving data boundaries, legal boundaries, and production-system boundaries.

Cernify is not another patent search wrapper. It is a product-evidence operating layer for robotics FTO preparation.

The public demo uses public or synthetic data only, avoids customer materials, and does not provide legal advice or infringement conclusions. It gives product teams, engineering teams, and patent counsel a shared map of what is known, what is inferred, what is missing, and where review should focus.

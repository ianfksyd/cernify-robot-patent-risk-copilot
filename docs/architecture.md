# Architecture

Cernify Robot Patent Risk Copilot demonstrates a public, schema-bound workflow:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

## Layers

1. Product evidence
   Public-reference or synthetic product images, specs, videos, manuals, or patent drawings.

2. Component graph
   A structured representation of visible modules and patent-sensitive subcomponents.

3. Evidence graph
   Links from components to observable facts, reasonable inferences, and evidence gaps.

4. Patent-risk map
   Demo-only mapping from technical features to patent candidate placeholders and risk factors.

5. Report artifact
   A sample evidence report for legal and product review workflows.

## Public Demo Boundary

This repository contains only public demo schemas, examples, and documentation.
It does not include production retrieval, ranking, FTO reasoning, customer data,
or internal Cernify APIs.


# Sample Robot FTO Evidence Report

Project: Cernify Robot Patent Risk Copilot  
Case: Public humanoid robot demo  
Status: Demo-only sample report

## Legal Disclaimer

This report is for demonstration and research workflow purposes only. It is not
legal advice, not an infringement determination, not a validity opinion, and not
a freedom-to-operate legal opinion.

## Scope

This sample report demonstrates how Cernify can organize robot product evidence
into a structured patent-risk workflow:

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

## Product Evidence

The public repository does not include full third-party source videos or
keyframe image files. Source media is referenced only through
`source_video_reference.md`.

## Component Summary

| Component | Evidence Status | Review Note |
| --- | --- | --- |
| Head perception module | Observable | Visible external module in public-reference evidence |
| Joint actuation module | Observable | Visible joint layout supports component analysis |
| Sensor fusion function | Inferred | Requires technical verification |

## Patent-Risk Summary

| Component | Demo Risk Level | Main Evidence Gap |
| --- | --- | --- |
| Head perception module | Medium | Sensor fusion implementation not confirmed |
| Joint actuation module | Medium | Supplier and control parameters not confirmed |

## Evidence Gaps

- Internal sensor fusion algorithm is not directly observable from public-reference evidence.
- Motor supplier, reducer type, and control parameters are not confirmed.
- Patent candidates are placeholders and require jurisdiction-specific legal review.

## Next Review Steps

1. Confirm product evidence sources and media rights.
2. Replace placeholder patent candidates with counsel-reviewed search results.
3. Create claim charts outside this public demo repository if authorized.
4. Obtain technical verification for inferred algorithmic features.


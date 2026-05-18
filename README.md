# Cernify Robot Patent Risk Copilot

Cernify turns robot product evidence into an interactive overseas patent risk map.

## Demo

- Live demo: TBD public static demo page or public demo video.
- Submission: UCWS 2026
- Track: Application

## What This Repository Includes

This repository contains the public UCWS demo layer for Cernify Robot Patent Risk Copilot:

- Capability schemas
- Synthetic and public-reference examples
- Sample component graphs
- Sample evidence graphs
- Sample patent-risk maps
- Sample FTO evidence reports
- Public documentation for the workflow

## What This Repository Does Not Include

This repository does not include Cernify's production platform, patent retrieval system, FTO reasoning engine, private datasets, customer workspaces, internal APIs, authentication system, billing system, deployment infrastructure, or production model prompts.

## Capability Flow

```text
product evidence -> component graph -> evidence graph -> patent-risk map -> report artifact
```

## Public Repository Scope

This repository open-sources the Cernify UCWS demo layer only. The production Cernify platform and proprietary patent-risk engine remain closed-source.

See:

- [PUBLIC_BOUNDARY.md](PUBLIC_BOUNDARY.md)
- [LEGAL_DISCLAIMER.md](LEGAL_DISCLAIMER.md)
- [docs/media_rights.md](docs/media_rights.md)

## Third-Party Media

Full third-party source videos are not included in this repository. Keyframe images are also omitted in the first release.

Third-party robot images, product videos, video frames, screenshots, logos, product names, and trademarks remain owned by their respective rights holders. Unless explicitly stated otherwise, they are not covered by this repository's open-source license.

## Repository Contents

```text
capabilities/   UCWS-ready capability manifests and sample inputs/outputs
docs/           Architecture, data policy, media rights, and demo story
examples/       Public-reference or synthetic demo outputs
evidence-packs/ Evidence package outputs and source reference templates
reports/        Sample FTO evidence reports
screenshots/    Screenshot review notes; no third-party screenshots by default
```

## Legal Disclaimer

The sample outputs, patent-risk maps, evidence reports, and FTO-related examples are for demonstration and research workflow purposes only.

They are not legal advice, not an infringement determination, not a validity opinion, not a freedom-to-operate legal opinion, and not a substitute for review by qualified patent counsel in the relevant jurisdiction.

## License

See [LICENSE](LICENSE) and [NOTICE](NOTICE). The license applies only to original files in this repository. It does not grant rights to Cernify trademarks, hosted services, proprietary datasets, production systems, or third-party media.


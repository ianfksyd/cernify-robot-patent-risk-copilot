# Security Policy

## Reporting Security Issues

Do not open public issues containing secrets, credentials, private URLs, customer
data, or internal system details.

For this UCWS demo repository, report security concerns privately to the project
maintainer.

## Public Repository Rules

Do not commit:

- `.env` files
- API keys, tokens, cookies, JWTs, private keys, or certificates
- Customer files, customer screenshots, customer reports, or customer workspace URLs
- Production API routes, request payloads, logs, model traces, prompts, or database schemas
- HAR files, network panel exports, console screenshots, or unredacted error logs
- Full third-party source videos or large keyframe dumps

If a secret is ever committed, rotate the secret and create a new clean public
repository instead of relying only on file deletion.


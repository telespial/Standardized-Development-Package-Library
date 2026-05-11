# Standardized Development Package (SDP)

Standardized Development Package (`SDP`) defines the hardware-and-firmware documentation contract for EmbeddedX development workflows.

It standardizes how a semiconductor manufacturer or platform provider can publish a reusable board package that includes required engineering context for firmware and AI-assisted embedded development.

An `SDP` package can include or reference:
- silicon datasheets and reference manuals
- register/programming references
- board schematics and BOM/assembly references
- peripheral/sensor/display/network component documentation
- firmware sample-code entry points
- SDK notes and validation guidance

`SDP` is the package layer that sits between board-level hardware knowledge and AI-assisted firmware coding workflows.

## v1 Goals

Version `1` of the package contract is optimized for practical bring-up and reuse:
- establish required core documentation for each board family
- define optional component placeholders for extension workflows
- standardize source-link and local-file attachment patterns
- support export/import portability across projects and teams
- enable team-safe sharing of board context for AI-assisted coding

## Relationship To Other Specifications

- `Embedded-Intelligence-Package-Specs` — umbrella ecosystem reference
- `EIP` — embedded intelligence/model package contract
- `MRD` / `MRC` / `MDP` — complementary structure and model contracts
- `EmbeddedX Client` — UI import/export and workflow consumption
- `EmbeddedX Server` — policy, orchestration, and future server-authoritative SDP logic

`SDP` covers board, silicon, and component documentation context.
`EIP` covers model/runtime packaging context.
Both are intended to interoperate in one end-to-end embedded workflow.

## Repository Layout

- `index.json` — machine-readable catalog used by EmbeddedX catalog import
- `vendors/<vendor>/<board>/<sample>/package.sdp.json` — package manifests
- `vendors/<vendor>/<board>/<sample>/README.md` — package-specific usage and component overview

## v1 Core Rules

An `SDP` package must:
- declare `packageType: standardized_developer_package`
- describe board/vendor/import-root metadata
- define `includes` capability flags
- define placeholders for required and optional documentation artifacts
- allow reference links and local-path linkage during project execution

## Why SDP Matters

`SDP` provides a standardized mechanism for semiconductor manufacturers and platform teams to deliver complete board-development context in one portable package.

It also allows end users to configure, save, and share board-specific documentation and component mappings for use with AI-assisted firmware coding systems.

This reduces repeated setup work, improves consistency, and accelerates project bring-up across teams.

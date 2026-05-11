# EmbeddedX Standardized Development Package Library

Central catalog for published EmbeddedX Standardized Development Packages (SDP).

## Catalog File

The client imports from:

- `index.json`

Schema:

- `version` (number)
- `updatedAt` (UTC ISO timestamp)
- `entries` (array)

Each entry should include:

- `id` (stable slug)
- `vendor`
- `board`
- `sample`
- `sdpUrl` (raw GitHub URL to `.sdp.json`) and/or `bundleUrl` (GitHub URL to `.zip`)
- optional `tags` (string array)

## Recommended Repo Layout

- `vendors/<vendor>/<board>/<sample>/package.sdp.json`
- `vendors/<vendor>/<board>/<sample>/bundle.zip`

## Publishing Workflow

1. Export from EmbeddedX Client:
   - Framework Only (`.sdp.json`) and optionally
   - Library and Framework (`.zip`)
2. Commit files under `vendors/...`
3. Add/refresh corresponding `entries[]` in `index.json`
4. Update `updatedAt`
5. Commit and push

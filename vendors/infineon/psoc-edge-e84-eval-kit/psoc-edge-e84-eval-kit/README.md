# Standardized Development Package (SDP): Infineon PSoC Edge E84 Eval Kit

Infineon PSoC Edge E84 Eval Kit `SDP` defines a standardized board package for EmbeddedX firmware and AI-assisted development workflows.

It captures required hardware/firmware documentation and optional component references in one reusable manifest so teams can import, maintain, and share board context consistently.

## Package Summary

- Vendor: `Infineon`
- Board: `PSoC Edge E84 Eval Kit`
- Package version: `0.1`
- Import root: `library/vendors/infineon/psoc-edge-e84-eval-kit`
- Spec URL: `https://github.com/telespial/Standardized-Developer-Package-Specs`

## v1 Goals For This Package

- establish minimum required silicon docs for safe bring-up
- provide optional placeholders for board and component expansion
- include sample-code placeholders for AI-assisted coding flows
- support team portability through import/export workflows

## Documentation Scope Covered

This SDP includes or references:
- silicon docs: datasheet, reference-manual, register/programming references
- board docs: user-guide, quick-start, release-notes, schematic, BOM/assembly references
- component docs: sensor/audio/network/display placeholders
- sample code placeholders and reference links

## Component Overview

- Board:
  - KIT_PSE84_EVAL base board
- Silicon:
  - PSoC Edge E8x family
  - MOD_PSE84_SOMS2 E84 SOM
- Sensors:
  - BMI270
  - BMM350
- Audio:
  - IM73D122V01XTMA1
  - IM73A135V01XTSA1
  - MCABS-247-RC speaker
- Network:
  - LAN8710AI
- Display:
  - Waveshare 4.3-inch DSI + FT5406
  - Waveshare 7.0-inch DSI + GT911
  - EK79007AD3 10.1-inch TFT + ILI2511
- Sample code:
  - EdgeAI Smart Pong Demo

## Package Metrics

- Total placeholders: `39`
- Required placeholders: `2`
- Reference links: `1`

Includes enabled:
- datasheets
- schematics
- bom
- sampleCode
- sdkNotes
- validation

## AI-Assisted Workflow Value

For semiconductor and platform delivery:
- standardizes required board-development artifacts in one package
- reduces ambiguity in firmware bring-up requirements

For end users and teams:
- supports configuring, saving, and sharing board-specific documentation and component context
- improves repeatability for AI-assisted firmware coding systems

## Files

- `package.sdp.json` — canonical SDP manifest for import/export.

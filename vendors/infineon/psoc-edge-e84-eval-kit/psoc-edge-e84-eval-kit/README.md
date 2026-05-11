# PSoC Edge E84 Eval Kit SDP

## Function

Standardized Development Package (SDP) scaffold for Infineon PSoC Edge E84 evaluation workflows in EmbeddedX.

This package provides a structured documentation and sample-code placeholder map so teams can:

- track required silicon docs (datasheet + reference manual),
- attach board/component collateral over time,
- keep reusable reference links with the package,
- and bootstrap sample-code linkage for EdgeAI demo flows.

## Dev Kit

- Vendor: Infineon
- Board: PSoC Edge E84 Eval Kit
- Package version: 0.1
- Import root: `library/vendors/infineon/psoc-edge-e84-eval-kit`

## Components Used

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
- Sample Code:
  - EdgeAI Smart Pong Demo

## Overview

- Total placeholders: 39
- Required placeholders: 2
- Reference links: 1
- Includes flags enabled in this SDP:
  - datasheets
  - schematics
  - bom
  - sampleCode
  - sdkNotes
  - validation

## Files

- `package.sdp.json`: Primary SDP manifest for import/export.

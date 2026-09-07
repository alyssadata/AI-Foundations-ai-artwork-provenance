# AI Foundations | AI Artwork Provenance

This repository preserves provenance records for AI-assisted artwork created through Alyssa Solen's concepts, art direction, iteration, selection, and final approval.

The purpose is to preserve more than a generic `AI-generated` label. Records document the creation chain and the surviving evidence around it: prompts, models, iterative changes, creative direction, recovered account-history screenshots, related explorations, and final or archival assets.

## Repository structure

- `artwork/` — artwork files and provenance-bearing screenshots
- `artwork-provenance/` — YAML provenance records for individual works or related creative series
- `metadata-template.yaml` — reusable machine-readable template
- `metadata-template.md` — short human-readable guide to the YAML format

## Provenance records

A stable ID such as `ART-001` can represent either:

- one specific artwork, or
- a related creative lineage / exploratory series when several files clearly belong together.

A grouped record does **not** have to claim that every image came from the same generation job. The relationship can instead be recorded as a shared concept, experiment, or development line.

Records can include:

- title or working label
- exact or approximate creation period
- concept, prompt, and art direction
- generation provider/tool/model when recoverable
- iteration or lineage notes
- recurring creative elements
- one or more primary provenance artifacts
- repository paths, file sizes, and GitHub blob SHAs
- SHA-256 content hashes when available
- verification status and method

## Provenance-bearing screenshots

For recovered historical artwork, a platform-history screenshot may be more useful than a later standalone download because it can preserve the artwork together with contextual evidence such as the prompt, model version, settings, account history, or relative age marker.

Those screenshots may therefore be treated as **primary provenance artifacts**. A standalone image file is optional unless it adds useful evidence or preserves the final artwork separately.

## Archival uncertainty

Not every historical field can be recovered years later. Unknown information can remain `null`, approximate years can be labeled as approximate, and exact dates are not asserted when the surviving evidence does not support them.

The archive favors preserved evidence over reconstructed certainty.

## Principle

The record preserves the creative trajectory rather than reducing the artwork to the tool that participated in generation.

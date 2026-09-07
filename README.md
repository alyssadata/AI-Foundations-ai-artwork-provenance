# AI Foundations | AI Artwork Provenance

This repository preserves provenance records for AI-assisted artwork created through Alyssa Solen's concepts, art direction, iteration, selection, and final approval.

The purpose is to preserve more than a generic `AI-generated` label. Each record documents the creation chain: what the artwork began as, which tools assisted generation, which changes were directed across iterations, which creative elements define the piece, and which final asset belongs to that record.

## Repository structure

- `artwork/` — final artwork assets
- `artwork-provenance/` — one YAML provenance record per artwork
- `metadata-template.yaml` — reusable machine-readable template
- `metadata-template.md` — short human-readable guide to the YAML format

## Provenance record

Each artwork receives a stable ID such as `ART-001` and its own `.yaml` file. A record can include:

- title and creation date
- concept and art direction
- generation provider/tool
- generation or editing method
- iteration lineage
- recurring creative elements
- selection and final approval
- final asset filename/path
- SHA-256 file hash when available

Not every field has to be known immediately. Missing information can remain `null` and be added later without changing the earlier provenance history.

## First record

`ART-001` documents **The Source**, a tarot-card artwork developed through iterative image generation and editing on September 7, 2026.

## Principle

The record preserves the creative trajectory rather than reducing the artwork to the tool that participated in generation.

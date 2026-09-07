# How the YAML record works

YAML is structured plain text. You do not need to learn much of it to use this repository.

- `field: value` stores one piece of information.
- Indented lines belong to the field above them.
- Lines beginning with `-` are list items.
- `null` means the information has not been recorded yet.
- Quotes keep titles, dates, and descriptive text unambiguous.

The reusable machine-readable template is [`metadata-template.yaml`](./metadata-template.yaml).

## One artwork or a related series

A provenance record can represent either one artwork or a related group of creative experiments.

For a single work, use a title such as:

`ART-001-the-source.yaml`

For several related screenshots or variations, use one series record such as:

`ART-003-early-self-generation.yaml`

The grouped record can list several files under `primary_artifacts`. Grouping them does not mean they must all be from the exact same generation job. Use the `relationship` section to say whether they share a concept, experiment, iteration line, or other creative relationship.

## Provenance-bearing screenshots

Historical platform screenshots can be treated as primary provenance artifacts when they preserve useful context such as:

- the generated artwork
- prompt text
- model version
- generation settings
- account-history placement
- relative age or date markers

A later standalone download is optional when the screenshot carries stronger provenance information.

## Approximate historical dates

When exact dates cannot be recovered, do not invent them. Use an approximate year or period and explain the basis. Fields can remain `null` when the evidence is insufficient.

## Integrity fields

For each repository artifact, a record may preserve:

- `repository_path` — where the file lives in this repository
- `filename` — the exact filename
- `file_size_bytes` — the exact file size
- `github_blob_sha` — GitHub's blob identifier for the repository object
- `sha256` — a portable cryptographic hash of the file bytes when available
- `verification` — whether and how the record was checked

You do not need to fill every field immediately. The archive can become more precise later without pretending that missing historical information was known earlier.

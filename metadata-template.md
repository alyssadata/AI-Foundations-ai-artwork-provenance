# How the YAML record works

YAML is structured plain text. You do not need to learn much of it to use this repository.

- `field: value` stores one piece of information.
- Indented lines belong to the field above them.
- Lines beginning with `-` are list items.
- `null` means the information has not been recorded yet.
- Quotes keep titles, dates, and descriptive text unambiguous.

The reusable machine-readable template is [`metadata-template.yaml`](./metadata-template.yaml).

For each finished artwork, copy that structure into `artwork-provenance/` and give the record its own ID, for example:

`ART-001-the-source.yaml`

The YAML preserves the creation chain: the concept, human art direction, generation assistance, iterative changes, recurring creative elements, selection, final approval, and the final asset tied to the record.

## Asset integrity fields

When the final artwork is in the repository, the record can also preserve:

- `repository_path` — where the artwork lives in this repository
- `filename` — the exact asset filename
- `file_size_bytes` — the exact file size
- `github_blob_sha` — GitHub's blob identifier for the repository object
- `sha256` — a cryptographic hash of the actual file bytes
- `verification` — whether and how the recorded asset was checked

The GitHub blob SHA and SHA-256 serve different purposes, so both may be recorded. The SHA-256 is the portable content-integrity hash for the artwork itself.

You do not need to fill every field immediately. Unknown or not-yet-recorded values can remain `null` until they are available.

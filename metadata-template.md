# How the YAML record works

YAML is just structured plain text. You do not need to learn much of it to use this repository.

- `field: value` stores one piece of information.
- Indented lines belong to the field above them.
- Lines beginning with `-` are list items.
- `null` means the information has not been recorded yet.
- Quotes keep titles, dates, and descriptive text unambiguous.

The reusable machine-readable template is [`metadata-template.yaml`](./metadata-template.yaml).

For each finished artwork, copy that structure into `artwork-provenance/` and give the record its own ID, for example:

`ART-001-the-source.yaml`

The YAML is intended to preserve the creation chain: the concept, human art direction, generation assistance, iterative changes, recurring creative elements, selection, final approval, and—when available—the final file path and cryptographic hash.

You do not need to fill every field immediately. Unknown or not-yet-recorded values can remain `null` until they are available.

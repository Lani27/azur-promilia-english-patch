# Release contract

`channel.json` is the public update pointer. Every change increments its monotonic `sequence`; existing revision numbers are never reused with different metadata.

The channel declares independent `minimum_patcher`, `minimum_engine`, and `required_capabilities` fields. `latest_patcher` is informational and never triggers an update notice. Raising `minimum_patcher` is reserved for compatibility or a necessary fix, explained in `reason`.

A ready channel points to one immutable, versioned GitHub release archive. `english-data.zip` contains exactly:

- `english.catalog.json.gz`: English, exact Japanese-source hashes, logical context identities, normalization data, and catalog metadata.
- `mapping.json`: versioned declarations for supported parsers. Native dispatch locations and codec-field references are bound to an exact installed binary hash. The package contains no code or codec secrets.

The channel records each member's size and SHA-256, plus the complete archive identity. The client validates the downloaded files before atomically activating them. Failed downloads preserve the previous compatible cache. A known required patcher fix remains required while offline.

Table names, row IDs and string offsets are discovered locally. New tables or moved IDs within supported formats do not require executable changes. A new native binary can receive a new verified mapping profile through data; an unsupported instruction or layout requires an engine implementation change.

Releases start as drafts. The publisher checks the uploaded asset's GitHub-reported digest before publishing the release, then advances the channel with a compare-and-swap update. Failed publication leaves the existing channel intact. Release assets are never overwritten in place.

Until full translation and validation complete, the channel has `state: "preparing"` and no data payload.

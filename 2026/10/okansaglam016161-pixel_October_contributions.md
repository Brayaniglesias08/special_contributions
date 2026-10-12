# okansaglam016161-pixel's October Contributions

A summary of contributions by okansaglam016161-pixel in October 2026:

- Reported a bug in the `tari-ootle` indexer's substate cache to the Tari team.
- The report showed that the cache turns every null in a cached component state into an empty array. `Value::Null` was serialized through `serialize_unit`, which `tari_bor::serde_codec` encodes as an empty array (`0x80`), so an `Option::None` field reads back as `[]`.
- Consequence: a dry run against a component with an `Option::None` field works on the first, uncached fetch, then fails with an `EngDcdFail` decode error once the corrupted copy is served from the cache. Provided the root cause, an offline reproduction of the codec round trip, and live dry runs showing the failure on a caching indexer.
- The fix was implemented separately by @sdbondi in `tari-project/tari-ootle#2870`. The contribution is tracked in `tari-project/special_contributions#136`.

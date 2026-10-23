# Security Reports — October 2026

Reported by [@m4r1m0](https://github.com/m4r1m0).

## Report 1 — GHSA-38xx-4h6j-jmr3

Messaging handler: no read timeout — stalled inbound streams pin task capacity and prevent connection reaping.

The report showed that messaging handler: no read timeout — stalled inbound streams pin task capacity and prevent connection reaping. The fix was applied by the Tari team in `tari-ootle#2770`.

Tracked by `tari-project/special_contributions#60`.

## Report 2 — GHSA-7vhp-937q-mc4w

Confidential transfer proofs with reveal amount are always invalid.

The report showed that confidential transfer proofs with reveal amount are always invalid. The fix was applied by the Tari team in `tari-ootle#2824`.

Reported by email to the Tari security team.

Tracked by `tari-project/special_contributions#153`.

## Report 3 — issue #159

Validator node shutdown via non-numeric filter in get_filtered_blocks_count.

The report showed that validator node shutdown via non-numeric filter in get_filtered_blocks_count. The fix was applied by the Tari team in `tari-ootle#2897`.

Reported by email to the Tari security team.

Tracked by `tari-project/special_contributions#159`.

## Report 4 — issue #161

Duplicate council keys halve effective m-of-n threshold.

The report showed that duplicate council keys halve effective m-of-n threshold. The fix was applied by the Tari team in `tari-ootle#2851`.

Reported by email to the Tari security team.

Tracked by `tari-project/special_contributions#161`.

## Report 5 — issue #165

Unauthenticated webauthn.start_auth session accumulation causes memory growth and quadratic CPU in walletd.

The report showed that unauthenticated webauthn.start_auth session accumulation causes memory growth and quadratic CPU in walletd. The fix was applied by the Tari team in `tari-ootle#2899`.

Reported by email to the Tari security team.

Tracked by `tari-project/special_contributions#165`.

## Report 6 — issue #203

RPC sessions have no idle timeout, silent sessions pin validator RPC pool.

The report showed that rPC sessions have no idle timeout, silent sessions pin validator RPC pool. The fix was applied by the Tari team in `tari-ootle#2816`.

Reported by email to the Tari security team.

Tracked by `tari-project/special_contributions#203`.

## Report 7 — GHSA-rr2h-gv24-pqxh

Malicious indexer crashes the wallet daemon via unwraps on substituted substate data.

The report showed that malicious indexer crashes the wallet daemon via unwraps on substituted substate data. The fix was applied by the Tari team in `tari-ootle#2813`.

Tracked by `tari-project/special_contributions#208`.

## Report 8 — GHSA-fgff-j3q5-7x83

Free validator log flood via oversized template panic messages (error level, no fee, no log-level dependency).

The report showed that free validator log flood via oversized template panic messages (error level, no fee, no log-level dependency). The fix was applied by the Tari team in `tari-ootle#2884`.

Tracked by `tari-project/special_contributions#209`.

## Report 9 — GHSA-pj47-wg83-jrjr

Confidential.create_output_proof produces undecryptable, unspendable outputs.

The report showed that confidential.create_output_proof produces undecryptable, unspendable outputs. The fix was applied by the Tari team in `tari-ootle#2946`.

Tracked by `tari-project/special_contributions#214`.

## Report 10 — GHSA-q46j-2mj8-wvqp

Debug log flood: per-call `tari_debug` budget lets one transaction write ~7 GiB of validator logs for ~0.25 tTARI.

The report showed that debug log flood: per-call `tari_debug` budget lets one transaction write ~7 GiB of validator logs for ~0.25 tTARI. The fix was applied by the Tari team in `tari-ootle#2949`.

Tracked by `tari-project/special_contributions#216`.

## Report 11 — GHSA-h7r6-f76r-8vc5

Burn-rate governance: stale locked epoch bypasses the activation lead time and rewrites the resolvable epoch window.

The report showed that burn-rate governance: stale locked epoch bypasses the activation lead time and rewrites the resolvable epoch window. The fix was applied by the Tari team in `tari-ootle#2952`.

Tracked by `tari-project/special_contributions#226`.

## Report 12 — GHSA-2gv4-x4gj-3p78

Walletd signs with caller-named mask keys: a read-only RPC leaks the blinding factors that hide confidential/stealth output values.

The report showed that walletd signs with caller-named mask keys: a read-only RPC leaks the blinding factors that hide confidential/stealth output values. The fix was applied by the Tari team in `tari-ootle#2960`.

Tracked by `tari-project/special_contributions#228`.

## Report 13 — GHSA-r5q2-hhx4-px6p

Unbounded missing-transactions response: one tiny request pins a validator's consensus worker (up to ~1.31 GB encoded per request).

The report showed that unbounded missing-transactions response: one tiny request pins a validator's consensus worker (up to ~1.31 GB encoded per request). The fix was applied by the Tari team in `tari-ootle#2962`.

Tracked by `tari-project/special_contributions#230`.

## Report 14 — GHSA-2pm9-q6j8-qrh8

A peer can pin gigabytes of validator memory: `get_substate_batch` buffers the whole response before streaming and bounds only its item count.

The report showed that a peer can pin gigabytes of validator memory: `get_substate_batch` buffers the whole response before streaming and bounds only its item count. The fix was applied by the Tari team in `tari-ootle#2966`.

Tracked by `tari-project/special_contributions#232`.

## Report 15 — GHSA-58hr-fqpx-8qcc

Unauthenticated peer forces an unbounded, unaccounted full-history state scan on a validator (`sync_state` work is decoupled from its response and from the peer's liveness).

The report showed that unauthenticated peer forces an unbounded, unaccounted full-history state scan on a validator (`sync_state` work is decoupled from its response and from the peer's liveness). The fix was applied by the Tari team in `tari-ootle#2967`.

Tracked by `tari-project/special_contributions#241`.

## Report 16 — GHSA-q278-wcqg-x39q

Malicious indexer aborts the wallet with one HTTP 304: the UTXO stream client unwraps a `None` status error.

The report showed that malicious indexer aborts the wallet with one HTTP 304: the UTXO stream client unwraps a `None` status error. The fix was applied by the Tari team in `tari-ootle#3023`.

Tracked by `tari-project/special_contributions#276`.

## Report 17 — GHSA-mxc7-fprj-8xq2

Foreign proposal notification from an unrelated committee suppresses the honest notification, so the block is never fetched from the committee that holds it.

The report showed that foreign proposal notification from an unrelated committee suppresses the honest notification, so the block is never fetched from the committee that holds it. The fix was applied by the Tari team in `tari-ootle#3025`.

Tracked by `tari-project/special_contributions#279`.

## Report 18 — GHSA-mm9x-928m-8gjc

Non-canonical confidential mask in a payer-crafted output panics the receiving wallet (persistent walletd crash loop).

The report showed that non-canonical confidential mask in a payer-crafted output panics the receiving wallet (persistent walletd crash loop). The fix was applied by the Tari team in `tari-ootle#3022`.

Tracked by `tari-project/special_contributions#280`.

## Report 19 — GHSA-m92m-fr3r-33v9

Unbounded SSE line/event buffering in the indexer client: a malicious indexer OOMs and CPU-burns the wallet.

The report showed that unbounded SSE line/event buffering in the indexer client: a malicious indexer OOMs and CPU-burns the wallet. The fix was applied by the Tari team in `tari-ootle#3035`.

Tracked by `tari-project/special_contributions#281`.

## Report 20 — GHSA-22mg-5wh7-3m6f

Template definition is deep-cloned on every resolve, giving a published template unmetered host CPU per transaction.

The report showed that template definition is deep-cloned on every resolve, giving a published template unmetered host CPU per transaction. The fix was applied by the Tari team in `tari-ootle#3041`.

Tracked by `tari-project/special_contributions#286`.

## Report 21 — GHSA-rrp6-34q3-56r8

Malicious indexer permanently poisons the wallet's stealth-UTXO scan cursor.

The report showed that malicious indexer permanently poisons the wallet's stealth-UTXO scan cursor. The fix was applied by the Tari team in `tari-ootle#3037`.

Tracked by `tari-project/special_contributions#287`.

## Report 22 — GHSA-mp6v-gfmj-r6xw

Post-invocation host charges push a fully executed main intent into the all-or-nothing reject path, refunding its fee.

The report showed that post-invocation host charges push a fully executed main intent into the all-or-nothing reject path, refunding its fee. The fix was applied by the Tari team in `tari-ootle#3040`.

Tracked by `tari-project/special_contributions#288`.

## Report 23 — GHSA-x9m4-9c4v-r385

Identify metrics retain every peer forever: unbounded memory growth on metrics-enabled validator/indexer nodes.

The report showed that identify metrics retain every peer forever: unbounded memory growth on metrics-enabled validator/indexer nodes. The fix was applied by the Tari team in `tari-ootle#3045`.

Tracked by `tari-project/special_contributions#290`.

## Report 24 — GHSA-vv2x-mqfw-p4xv

Indexer REST client parses an unbounded error body into `serde_json::Value`: a 61 MiB `500` response expands to ~2 GiB of wallet heap.

The report showed that indexer REST client parses an unbounded error body into `serde_json::Value`: a 61 MiB `500` response expands to ~2 GiB of wallet heap. The fix was applied by the Tari team in `tari-ootle#3058`.

Tracked by `tari-project/special_contributions#295`.

Technical details remain in each advisory, or with the Tari security team for reports made by email, until published.

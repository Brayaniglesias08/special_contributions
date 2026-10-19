# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: a block's transaction_merkle_root is quorum-signed but never recomputed from the block's commands, letting a Byzantine leader commit a false finalization/exclusion proof, tracked in `GHSA-c5rq-wmvm-qqwx`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#198`.

# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: cross-shard transactions can freeze user funds permanently because the non-cooperating-foreign-shard-group timeout/abort was never implemented, tracked in `GHSA-93fg-xrrm-gmcg`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#174`.

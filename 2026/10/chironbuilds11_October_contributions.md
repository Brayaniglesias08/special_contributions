# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: the validator node JSON-RPC allows unauthenticated, unbounded block pagination, enabling a remote DoS with a panic=abort amplifier, tracked in `GHSA-h759-f369-m2jv`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#177`.

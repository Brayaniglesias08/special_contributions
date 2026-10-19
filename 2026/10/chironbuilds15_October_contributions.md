# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: the 4 MiB aggregate transaction-output cap is never checked on the fee-intent-only commit path, letting one ordinary transaction commit up to roughly 1 GiB of state, tracked in `GHSA-hg3x-m3g3-vjq9`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#195`.

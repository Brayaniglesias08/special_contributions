# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: transaction admission and consensus validation enforce no fee sufficiency or minimum fee-rate, so dust-fee transactions are accepted, stored, proposed, and executed network-wide at zero cost, enabling unbounded mempool and execution DoS, tracked in `GHSA-vf6j-c5c9-gg9m`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#144`.

# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: the wallet derives its fee-swap input from unverified indexer pool reserves with no cap or confirmation, so a lying indexer can make a fee swap sell the user's entire token balance into an attacker-owned pool, tracked in `GHSA-mv6w-58hv-xv8r`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#143`.

# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: transactions are fully re-executed on every block they meet a deferrable soft-lock conflict with no fee ever charged, crowding out the per-block execution budget, tracked in `GHSA-gp95-gx5w-9545`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#215`.

# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: the engine compiles stored template binaries without re-checking them against the template address (a defence-in-depth gap), tracked in `ISSUE-2847`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#243`.

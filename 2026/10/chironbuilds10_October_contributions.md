# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: manifest identifiers resolve to different sources depending on argument vs. receiver position, letting a caller-supplied variable silently override a manifest's own binding, tracked in `GHSA-hf3w-78vr-3rj3`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#179`.

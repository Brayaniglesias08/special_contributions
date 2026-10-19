# chironbuilds's October Contributions

A summary of security contributions by chironbuilds in October 2026:

* Reported a security vulnerability in `tari-ootle`: the reservoir-sampling proposal batch selector decodes the entire ready transaction pool on every proposal regardless of the block budget, enabling network-wide liveness degradation, tracked in `GHSA-fc8p-764g-6r62`.
* The report included a root-cause analysis, a proof of concept where applicable, and a suggested fix. Testing was performed locally only; no shared network was touched.
* Coordinated through private disclosure; technical details remain in the advisory until it is published. This contribution is tracked in `tari-project/special_contributions#200`.

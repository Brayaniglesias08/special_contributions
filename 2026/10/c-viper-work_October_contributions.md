# c-viper-work's October Contributions

A summary of security contributions by c-viper-work in October 2026:

* Reported a security vulnerability in `tari-ootle`: `ResourceContainer::Confidential` revealed-change overflow against `locked_revealed_amount` and duplicate-commitment acceptance in `engine_types`, tracked in `GHSA-82jm-8fx9-mh39`. The report included a root-cause analysis, runnable regression tests, and a suggested fix; testing was performed locally only. Coordinated through private disclosure; the fix was applied by the Tari team in `tari-project/tari-ootle#3014`. This contribution is tracked in `tari-project/special_contributions#273`.
* Reported a security vulnerability in `tari-ootle`: `ootle-rs` `IndexerTrust::Verify` bypasses via unrequested batch substates, omitted account vaults, and unverified `get_resource` reads, tracked in `GHSA-4x6r-vhmx-g34f`. The report included a root-cause analysis, runnable regression tests, and a suggested fix; testing was performed locally only. Coordinated through private disclosure; the fix was applied by the Tari team in `tari-project/tari-ootle#3038`. This contribution is tracked in `tari-project/special_contributions#282`.

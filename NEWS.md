[19-08-25]

Retired traces: 1755530535, 1755530535 1755530728 1755530896 1755531000
1755531081 1755531179 1755531229 1755531322 1755531375 1755531419 1755531480

[18-08-25]

Updated the disputed reports table in `fuzz-reports/README.md` with additional  
**highly controversial** trace reports. Please review them **carefully and critically**.  
As often emphasized, GP is the single source of truth, avoid blindly matching against
the fuzzer's expected results.

[17-08-25]

Added comprehensive Disputes table to fuzz-reports/README.md showing test results
across all the fuzzed JAM implementations.
The table provides a clear overview of which reports cause failures or crashes for each team,
making it easier to track implementation conformance and identify problematic test cases.

Enhanced README.md with "Notes on Reports, Requests, and Contributions" section
to help set clear expectations for collaboration and support. This guidance aims
to make interactions more effective for everyone while keeping the project sustainable.

[15-08-25]

Highly disputed report: 1755248982 - All teams affected.
Possible reason: https://github.com/davxy/jam-conformance/issues/16#issuecomment-3190838048

Removed problematic reports from `archive`: 1754582958 1754725568 1754754058 1755184602

From now on, I will not continuously ping teams in their issue when new reports
are available. It is the team's responsibility to check their folder for any
new reports. Please leave a comment in the issue when an outstending report is
sorted/analyzed, including the reason for the failure. This reason will be added
to the archived report to help other teams and to speed up troubleshooting of
potential regressions. I will double-check the fix before moving the report to
the archive.

[14-08-25]

Archive of inter-team reports: [./fuzz-reports/archive]  
Teams are encouraged to review and execute one another's reports.

Target download script available at [./scripts/get_target.sh].
Target run script available at [./scripts/run_target.sh].
Target implementors are encouraged to submit a PR when repository locations
change or to enhance the script functionality.

Binary decoder script added at [./scripts/decode.py] for decoding JAM-encoded
binaries found in this repository. Requires https://github.com/davxy/jam-types-py.

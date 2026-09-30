# ChangJiangLab opportunity feed

This repository is an automated data mirror of the public ChangJiangLab
project aggregation API: https://xiangshanlab.shu.edu.pl/api/projects

Aggregation entries are not official announcements. Eligibility, deadlines,
fees, funding and application instructions must be verified on official project
pages. This mirror supports personal research opportunity screening.

Read `run_summary.json` to check freshness and collection status.
The separate `wechat/` folder contains public article metadata from the
ChangJiangLab WeChat account when the local subscription is configured.
Its `run_summary.json` reports subscription health; `archive/index.json`
lists incremental article batches. No WeRead credentials or article bodies
are published.
Read `latest/all_projects.json` for the initial snapshot, then
`archive/index.json` for the chronological history of successful batches.
For tools with file-size limits, use `latest/index.json` and its small parts.
Large incremental files also have part paths in the archive index.
Batch paths are repository-relative. Timestamps include an explicit UTC+08:00
offset. Projects retain their original IDs and include a public content hash.

The mirror does not contain local crawler state, personal configuration,
credentials, cookies or logs. Absence of new projects does not imply the source
was refreshed today: always check the latest successful collection time.

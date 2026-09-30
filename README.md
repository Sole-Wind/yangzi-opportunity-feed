# ChangJiangLab opportunity feed

The active feed is public article metadata from WeChat accounts subscribed
in the dedicated local source. It is collected twice weekly, on Tuesday
at 10:00 and Thursday at 16:00 Asia/Shanghai time. A separate screening
run should check the WeChat status before drawing conclusions.

The earlier ChangJiangLab project aggregation API snapshot is kept here as
historical reference. Its collection stopped on 2026-09-30 because the API
did not reflect recent WeChat articles. Do not treat its age as a current
collection failure or as evidence that there are no new opportunities.

Aggregation entries are not official announcements. Eligibility, deadlines,
fees, funding and application instructions must be verified on official project
pages. This mirror supports personal research opportunity screening.

Read `run_summary.json` to check freshness and collection status.
The `wechat/` folder contains public article metadata from the subscribed
accounts. `wechat/run_summary.json` includes per-account source health.
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

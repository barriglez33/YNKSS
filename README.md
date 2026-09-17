# Yankees News

GitHub-online-only RSS monitor for Yankees coverage.

Tracks 45 names from the supplied Yankees list.

Features:
- multilingual discovery using GDELT + Google News
- Yankees/MLB context filtering to reduce false positives
- automatic Spanish translation before RSS generation
- source included in every title, e.g. `[ESPN] Aaron Judge...`
- smart duplicate detection across publishers/languages
- only the most complete repeated version is kept
- alternate sources are preserved in `alternate_sources`
- master RSS plus individual RSS feeds
- GitHub Actions runs every hour at minute `:31`

Workflow:
`.github/workflows/update.yml`

Run manually:
**Actions → Update Yankees News RSS → Run workflow**

Generated:
- `docs/feed.xml`
- `docs/people/*.xml`
- `docs/index.html`
- `data/articles.json`

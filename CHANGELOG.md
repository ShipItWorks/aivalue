# Changelog

Public record of changes to aivalue, written from the product page on shipitworks.com. The source is private. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Release tags exist on the private repository's default branch.

## 2026-11-10 (release v0.3.0)

- 2026-11-10: Land PR #26 merged into main as 48ab047 (13 lane PRs included); no feature label changed this round. Tagged v0.3.0 at 48ab047.

Score 68 / 100 on our own rubric, scored 2026-11-10. Product page: https://shipitworks.com/apps/#aivalue

## 2026-11-08 (release v0.2.0)

- 2026-11-08: Score re-measured against main at 497c725 (tag v0.2.0): 68/100 on our own rubric, down from 72. Three of five features (calculators, catalog and database, backup and restore) now link a saved unit-test log from 2026-11-07 (58 tests, 0 failed, exit 0). Executive PDF export and the screens have no run log, so they are not tested yet.
- 2026-11-08: The Home screen button now reads 'Privacy & Methodology: no network permission declared' instead of 'no data leaves this device', and the Play kit drops 'Zero Cloud Collection' (PR #25, tag v0.2.0); no network capture exists, so traffic is not yet traced.
- 2026-11-08: CI on main now runs on the self-hosted runner (PR #24); the five latest main runs show success.

Score 68 / 100 on our own rubric, scored 2026-11-08. Product page: https://shipitworks.com/apps/#aivalue

## 2026-11-07 (release v0.1.1)

- The README and the in-app privacy copy now say only what was checked: the debug build declares no permissions (so no INTERNET), the release dependencies include no analytics, crash-reporting or ads library (a name match, not a network capture), and 58 unit tests pass (no device or PDF rendering coverage). Release v0.1.1.

Score 72 / 100 on our own rubric, scored 2026-11-01; no score or proof label changed in this update. Product page: https://shipitworks.com/aivalue/

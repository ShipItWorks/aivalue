# AI Value

Model AI ROI, P&L margins, Balance Sheet cash flow & 30-day adoption pilots.

**Score: 68 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-10; this record was updated 2026-11-10 from the [product page](https://shipitworks.com/apps/#aivalue).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Android. Not on Google Play yet.

## What works today

- 7 financial calculators (FinancialEngine) (Proven)
- Catalog + Room database load (Proven)
- JSON backup/restore (Proven)

## Not done yet

- Executive PDF export (Not tested yet)
- UI screens (Home, Explore, Calculators, Playbooks, Learn, Privacy) (Not tested yet)
- Executive PDF export: built, not tested yet. The device log on main (proof/executive-pdf-device.log) names lane commit f3b4cdc, which is not an ancestor of main, and checks only the header, trailer and size; the multi-page change (PR #12, landed in 48ab047) has no device run
- UI screens: not tested yet; no instrumented or UI run, no tracked screenshots
- Privacy: no permissions declared in the debug APK and no analytics library by name in release dependencies (2026-11-07 logs); no network capture, so runtime behaviour is not yet traced. README line 3 now says network traffic has not yet been captured (PR #23, landed in 48ab047)
- No signed release build and assembleRelease not run; the existing release APK is debug-key signed, so it cannot go to Play
- No user guide and no LICENSE on main (2026-11-10; CHANGELOG.md lists one, and PR #4 that carries it is open); root still holds ~20 stray chat-dump files and wrong-path duplicate catalog JSONs

## What changed

- 2026-11-10: Land PR #26 merged into main as 48ab047 (13 lane PRs included); no feature label changed this round. Tagged v0.3.0 at 48ab047.
- 2026-11-08: Score re-measured against main at 497c725 (tag v0.2.0): 68/100 on our own rubric, down from 72. Three of five features (calculators, catalog and database, backup and restore) now link a saved unit-test log from 2026-11-07 (58 tests, 0 failed, exit 0). Executive PDF export and the screens have no run log, so they are not tested yet.
- 2026-11-08: The Home screen button now reads 'Privacy & Methodology: no network permission declared' instead of 'no data leaves this device', and the Play kit drops 'Zero Cloud Collection' (PR #25, tag v0.2.0); no network capture exists, so traffic is not yet traced.
- 2026-11-08: CI on main now runs on the self-hosted runner (PR #24); the five latest main runs show success.
- 2026-11-07: The README and the in-app privacy copy now say only what was checked: the debug build declares no permissions (so no INTERNET), the release dependencies include no analytics, crash-reporting or ads library (a name match, not a network capture), and 58 unit tests pass (no device or PDF rendering coverage). Release v0.1.1.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (3:08)](https://shipitworks.com/aivalue/transcript/) · video on the [product page](https://shipitworks.com/apps/#aivalue)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#aivalue) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.

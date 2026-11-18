# AI Value

Model AI ROI, P&L margins, Balance Sheet cash flow & 30-day adoption pilots.

**Score: 68 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-11; this record was updated 2026-11-18 from the [product page](https://shipitworks.com/aivalue/).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Android. Not on Google Play yet.

## What works today

- 7 financial calculators (FinancialEngine) (Proven)
- Catalog + Room database load (Proven)
- JSON backup/restore (Proven)

## Not done yet

- Executive PDF export (Not tested yet)
- UI screens (Home, Explore, Calculators, Playbooks, Learn, Privacy) (Not tested yet)
- Executive PDF export: built. On 2026-11-18 a review ran ExecutivePdfInstrumentedTest on an Android 16 emulator at commit e5cafeb and it passed 5 of 5; it was not run on a phone in that review. The scorecard label for this feature stays at not tested yet until the scorecard is re-scored at that commit
- UI screens: not tested yet; no device run log of the screens was read. proof/ at 0d37284 holds emulator run logs added after 48ab047 (none added after 0f47543) that are listed for the owner and not scored here; tracked screenshots under floor/screen/ were not looked at (not verified 2026-11-11)
- Privacy: no permissions declared in the debug APK and no analytics library by name in release dependencies (2026-11-07 logs); no network capture, so runtime behaviour is not yet traced. README line 3 now says network traffic has not yet been captured (PR #23, landed in 48ab047)
- No signed release build and assembleRelease not run; the existing release APK is debug-key signed, so it cannot go to Play
- No user guide. A LICENSE file was added on main by PR #28 (ca8e567; on the tree at 0d37284, 2026-11-11; gh repo view reports licence key other and visibility PRIVATE; what it permits is not assessed here); at 0f47543 there was none (commit 9e10089 had removed it). Root still holds ~20 stray chat-dump files and wrong-path duplicate catalog JSONs

## What changed

- 2026-11-18: A review counted 122 unit tests in the source at commit e5cafeb; its Gradle unit-test run (testDebugUnitTest) exited 0, and the number of tests executed was not saved. The same review ran the executive PDF test on an Android 16 emulator: 5 of 5 passed. No feature label or score changed.
- 2026-11-11: Merged into the product: Home now offers a "Load example scenarios" button on an empty workspace that saves one example per calculator, built from the bundled use cases; a LICENSE file was added (the file says all rights are reserved; text in ev/aivalue-contents-LICENSE-0d37284.txt; the repository is private); and the proof scripts for the emulator checks were extended (PRs #43 and #28). This scorecard round did not run the app or the new test, and the automated check on this commit had not finished when read, so no feature label or score changed. Scorecard row: "UI screens (Home, Explore, Calculators, Playbooks, Learn, Privacy)" (works false, Not tested yet) is the row the Home button belongs to; the licence file and the proof scripts are not scored (no row covers them).
- 2026-11-11: Merged into the product, as its own change log lists them: a web version of the seven calculators (in the code, not hosted), report export as PDF, spreadsheet and slides, and a multi-year view with a sensitivity table. One of the automated checks failed on this commit and this scorecard round did not re-run them, so no feature label or score changed (PRs #33, #30 and #27).
- 2026-11-10: Land PR #26 merged into main as 48ab047 (13 lane PRs included); no feature label changed this round. Tagged v0.3.0 at 48ab047.
- 2026-11-08: Score re-measured against main at 497c725 (tag v0.2.0): 68/100 on our own rubric, down from 72. Three of five features (calculators, catalog and database, backup and restore) now link a saved unit-test log from 2026-11-07 (58 tests, 0 failed, exit 0). Executive PDF export and the screens have no run log, so they are not tested yet.
- 2026-11-08: The Home screen button now reads 'Privacy & Methodology: no network permission declared' instead of 'no data leaves this device', and the Play kit drops 'Zero Cloud Collection' (PR #25, tag v0.2.0); no network capture exists, so traffic is not yet traced.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (1:56)](https://shipitworks.com/aivalue/transcript/) · video on the [product page](https://shipitworks.com/aivalue/)

The demo voice is AI-generated (ElevenLabs, "Bella") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/aivalue/) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.

# AI Value

Model AI ROI, P&L margins, balance-sheet cash flow and 30-day adoption pilots.

**Score: 72 / 100** on the [ShipItWorks rubric](https://shipitworks.com/how-we-score/). Stage: Beta. As of 2026-11-02, from the [product page](https://shipitworks.com/apps/#aivalue).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Android. Not on Google Play yet.

## What works today

- 7 financial calculators (FinancialEngine)
- Catalog + Room database load
- JSON backup/restore

## Not done yet

- Executive PDF export still unproven: the instrumented test could not be re-run on 2026-11-01; a fresh installDebugAndroidTest is needed
- No UI/instrumented run of the app screens; no signed release build and no tracked screenshots, so it cannot go to Play
- assembleRelease not run; the existing release APK is debug-key signed
- No user guide; root still holds ~20 stray chat-dump files, and there are wrong-path duplicate catalog JSONs

## Demo

[Transcript of the demo (3:08)](https://shipitworks.com/aivalue/transcript/) · video on the [product page](https://shipitworks.com/apps/#aivalue)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README, and soon a CHANGELOG and LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#aivalue) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.

---
layout: default
title: Controlled review fixture v3
---

# Controlled review fixture v3

This directory contains Panel Pilot's current original App Review fixture. It demonstrates manual repository installation, authenticated APK identity, resource-backed extension settings, source browsing, chapter/page resolution, guided panel reading, and title-safety decisions without listing or endorsing a third-party catalogue.

Repository URL:

`https://raw.githubusercontent.com/ahibbert/panelpilot-public/main/review-fixture-v3/index.json`

The source exposes one allowed action-manga title plus two metadata-only safety cases. **Mature Safety Fixture** is tagged `Mature`, has no browse cover, and must be blocked until the app's mature non-graphic opt-in is enabled. **Graphic Safety Fixture** is tagged `Hentai`, has no browse cover or accessible chapters, and must remain blocked after opt-in. The APK deliberately throws if the host asks it for the graphic fixture's chapters, providing evidence that Panel Pilot classified details first.

The allowed and opted-in mature paths reuse Panel Pilot's original action-manga page over HTTPS. The safety cases contain no mature or graphic artwork.

## Published identity

- Package: `org.panelpilot.fixture`
- Version: `3.0.0` (`3`)
- APK SHA-256: `57071cf2e2d86737e44d1baa73107e6d60432905895c3bb2b48611c67c2ed454`
- Signing certificate SHA-256: `b095a74146ab120142027e7969e6ec0e85ee7f2ebe242e635a65dea95101afd1`
- Source commit: `a932c5eedb54a908e51d1a450975e8b0088b4a0c`
- Build run: `38145632996`

The APK is signed with Android signature schemes v2 and v3, preserves the v2 fixture's signing certificate, contains DEX bytecode and compiled string resources, and contains no native library. The generated [signer report](apksigner-report.txt) and [build provenance](build-provenance.txt) are published beside it.

This v3 fixture is immutable. Future changes must increment the repository version and package version code; its bytes, identity, or signing certificate must not be silently replaced.

The reused page remains governed by the original [artwork provenance](../review-fixture/ARTWORK.md).

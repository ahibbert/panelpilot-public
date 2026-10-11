---
layout: default
title: Controlled review fixture v4
---

# Controlled review fixture v4

This directory contains Panel Pilot's current original App Review fixture. It demonstrates manual repository installation, authenticated APK identity, resource-backed extension settings, source browsing, chapter/page resolution, guided panel reading, and title-safety decisions without listing or endorsing a third-party catalogue.

Repository URL:

`https://raw.githubusercontent.com/ahibbert/panelpilot-public/main/review-fixture-v4/index.json`

The source exposes one allowed action-manga title plus three coverless metadata-only safety cases. **Mature Safety Fixture** is tagged `Mature` and must be blocked until the app's mature non-graphic opt-in is enabled. **Graphic Safety Fixture** is tagged `Hentai`, and **Violence Safety Fixture** is tagged `Gore`; both must remain blocked after opt-in. The APK deliberately throws if the host asks it for either always-blocked fixture's chapters, providing evidence that Panel Pilot classified details first.

The allowed and opted-in mature paths reuse Panel Pilot's original action-manga page over HTTPS. The safety cases contain no mature, sexual, or violent artwork.

## Published identity

- Package: `org.panelpilot.fixture`
- Version: `4.0.0` (`4`)
- APK SHA-256: `0736ffbe0f891b73dd13b9872be55fba3e1eb79862bcaa5111d68dd7415e43ed`
- Signing certificate SHA-256: `b095a74146ab120142027e7969e6ec0e85ee7f2ebe242e635a65dea95101afd1`
- Source commit: `b604f445b9c370d87d1c88fc3e84d8a124acd8b6`
- Build run: `38149644958`

The APK is signed with Android signature schemes v2 and v3, preserves the v2/v3 fixture signing certificate, contains DEX bytecode and compiled string resources, and contains no native library. The generated [signer report](apksigner-report.txt) and [build provenance](build-provenance.txt) are published beside it.

This v4 fixture is immutable. Future changes must increment the repository version and package version code; its bytes, identity, or signing certificate must not be silently replaced.

The reused page remains governed by the original [artwork provenance](../review-fixture/ARTWORK.md).

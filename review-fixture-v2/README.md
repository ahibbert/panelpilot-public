---
layout: default
title: Controlled review fixture v2
---

# Controlled review fixture v2

This directory contains Panel Pilot's current original, non-adult App Review fixture. It demonstrates manual repository installation, authenticated APK identity, resource-backed extension settings, source browsing, chapter/page resolution, and guided panel reading without listing or endorsing a third-party catalogue.

Repository URL:

`https://raw.githubusercontent.com/ahibbert/panelpilot-public/main/review-fixture-v2/index.json`

The fixture exposes boolean, single-select, multi-select, text, and unsupported/read-only preference types. Its category, single-select title/summary, and option labels are loaded from authenticated APK resources. The source loads the original action-manga page published with the immutable v1 fixture over HTTPS.

## Published identity

- Package: `org.panelpilot.fixture`
- Version: `2.0.0` (`2`)
- APK SHA-256: `aebcdf9a35a96d8bacb5d8f560e792810472c18bd4b46f0442535ddc16658c4c`
- Signing certificate SHA-256: `b095a74146ab120142027e7969e6ec0e85ee7f2ebe242e635a65dea95101afd1`
- Source commit: `f7f5d634a88860008fc033edd0cacc6d6d58a36b`

The APK is signed with Android signature schemes v2 and v3, contains DEX bytecode and compiled string resources, and contains no native library. Its dedicated fixture-only signing identity is retained in encrypted CI secrets so future explicitly versioned fixtures can preserve certificate continuity. The generated [signer report](apksigner-report.txt) and [build provenance](build-provenance.txt) are published beside it.

This v2 fixture is immutable. Future changes must increment the repository version and package version code; its bytes, identity, or signing certificate must not be silently replaced.

The reused page remains governed by the original [artwork provenance](../review-fixture/ARTWORK.md).

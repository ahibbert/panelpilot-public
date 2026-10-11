# Controlled review fixture

This directory contains Panel Pilot's original, non-adult App Review fixture. It demonstrates the same user-supplied repository flow available in the app without listing or endorsing any third-party catalogue.

Repository URL:

`https://raw.githubusercontent.com/ahibbert/panelpilot-public/main/review-fixture/index.json`

The repository contains one Mihon-compatible source, two short chapter records, and an original action-manga page. The source runs through Panel Pilot's interpreter-only extension runtime and loads the page directly from this repository over HTTPS. The artwork and on-device panel detector provide a complete browse-to-guided-reading review path without a user account.

## Published identity

- Package: `org.panelpilot.fixture`
- Version: `1.0.0` (`1`)
- APK SHA-256: `c2bf2e6763722eff3bb4f495c187c6312418984e029beb4303c96d432bb1134d`
- Signing certificate SHA-256: `8d2c9a2fe0c658518263f703e7e08b2f3b0397a135aed7970353b18d8d14d83d`
- Source commit: `d5aaf5f1ce07f0e55a08b422e204967cf655effb`

The APK is signed with Android signature schemes v2 and v3 and contains DEX bytecode only—no native library. The generated [signer report](apksigner-report.txt) and [build provenance](build-provenance.txt) are published beside it.

This v1 fixture is immutable. Replacing its bytes, index identity, or signing certificate in place would violate the app's signer-continuity guarantee. Any future replacement must be published as a new explicitly versioned review fixture and must not silently update an installed package.

See [ARTWORK.md](ARTWORK.md) for the page's creation record and hash.

The same original page is also available as a deterministic, non-executable
[CBZ import fixture](files/) for the document-picker review path. It is
separate from the extension APK and can be read entirely offline after import.

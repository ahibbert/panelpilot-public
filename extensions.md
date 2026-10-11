---
layout: default
title: Extension policy
---

# Third-party extension metadata policy

Panel Pilot ships no extension catalogue and does not promote repositories. Users manually enter repository URLs and review each extension's package identity, signing certificate, requested network domains, version, language, and content classification before installation.

Unknown repositories are labelled unverified. A package is not installed until the app has downloaded a fresh signed safety policy, authenticated its APK signature and package name, checked its version and domains against that policy, and received explicit approval for its signing certificate and network domains. A certificate change requires removal and a new first-use review. Newly observed domains are blocked before transport and require another explicit review.

Signed-feed classifications for pornographic or graphically sexual material, gore/guro, prolonged graphic violence, and sadistic violence are always blocking. Mature and mixed-mature classifications require the local mature-content opt-in. Title metadata is classified before a remote cover, chapter list, or page can be loaded.

Panel Pilot's public extension index lists only explicitly versioned controlled review fixtures and the software metadata required for App Review. The current v3 fixture includes coverless metadata-only mature and always-blocked cases so reviewers can verify that title classification happens before chapter or page resolution. It does not provide a general third-party catalogue. A user can report an installed extension from the app after the metadata-only reporting service is enabled; reports never include comic pages or library history.

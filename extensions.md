---
layout: default
title: Extension policy
---

# Third-party extension metadata policy

Panel Pilot ships no extension catalogue and does not promote repositories. Users manually enter repository URLs and review each extension's package identity, signing certificate, requested network domains, version, language, and content classification before installation.

Unknown repositories are labelled unverified. A package is not installed until the app has downloaded a fresh signed safety policy, authenticated its APK signature and package name, checked its version and domains against that policy, and received explicit approval for its signing certificate and network domains. A certificate change requires removal and a new first-use review. Newly observed domains are blocked before transport and require another explicit review.

Panel Pilot's public extension index will list only controlled review fixtures and the software metadata required for App Review. It will not provide a general third-party catalogue. A user can report an installed extension from the app after the metadata-only reporting service is enabled; reports never include comic pages or library history.

---
layout: default
title: Extension policy
---

# Third-party extension metadata policy

Panel Pilot ships no extension catalogue and does not promote repositories. Users manually enter repository URLs and review each extension's package identity, signing certificate, requested network domains, version, language, and content classification before installation.

Unknown repositories are labelled rights-unverified. A package is not installed until the app has downloaded a fresh signed safety policy, authenticated its APK signature and package name, checked its version and domains against that policy, and received explicit approval for its signing certificate, network domains, and lawful-use acknowledgement. First installs remain disabled until a separate enable confirmation. A certificate change requires removal and a new first-use review. Newly observed domains are blocked before transport and require another explicit review. Package or repository identity verification must not be described as rights verification.

Users may manually install a technically valid extension even when its rights basis has not been reviewed. By default, an unverified extension is excluded from cross-source discovery and cannot create permanent offline downloads. A positive rights decision requires recorded operator and repository/package evidence; shared-domain status alone cannot confer it. Offline copying requires a separate explicit signed permission, silence means no permission, and any matching denial wins.

The signed policy may mark a repository, package, signer, or domain `under-review` or `blocked` for rights reasons. Those states pause networking without uninstalling the package or searching or deleting local user files. Signing establishes package identity only; it is never evidence that an extension operator or dynamic source is authorised to reproduce every item it exposes.

Signed-feed classifications for pornographic or graphically sexual material, gore/guro, prolonged graphic violence, and sadistic violence are always blocking. Mature and mixed-mature classifications require the local mature-content opt-in. Title metadata is classified before a remote cover, chapter list, or page can be loaded.

Panel Pilot's public extension index lists only explicitly versioned controlled review fixtures and the software metadata required for App Review. The current v4 fixture uses original CC0 artwork and includes coverless metadata-only mature, graphic-sexual, and prohibited graphic-violence cases so reviewers can verify that title classification happens before chapter or page resolution and that mature opt-in never unlocks always-blocked content. It does not provide a general third-party catalogue. A user can report an installed extension from the app after the metadata-only reporting service is enabled; reports never include comic pages or library history.

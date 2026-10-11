# Panel Pilot privacy policy — pre-release draft

Status: published for internal testing and review preparation. Specialist review, final contact details, and an effective date are still required before public distribution.

Panel Pilot is local-first and does not include advertising, tracking, analytics, or a Panel Pilot account. Comic pages, imported archives, downloads, panel detections, corrections, Moments, reading history, statistics, and source-reliability observations remain on the device unless the user explicitly exports or shares them.

When a user configures a third-party extension, requests go directly from the device to the domains shown in the extension trust screen. Those services apply their own privacy policies and may observe normal network data such as the IP address, requested resource, and headers required by the source. Panel Pilot does not proxy those requests.

The optional MangaBaka connection sends requests directly to MangaBaka. Its personal access token is stored in the iOS Keychain. Searching to link a title sends the entered title query. If progress sync is enabled, Panel Pilot sends only the linked MangaBaka series ID, reading status, and completed chapter number. It does not send comic pages, source URLs, Moments, reading time, or unlinked library entries.

User-initiated extension safety reports contain only the extension or package identity, source identity if relevant, version, signing-certificate hash, relevant domain, selected reason, and optional comment. They never attach comic pages, title or chapter names, library data, search history, or reading history. Safety reporting remains disabled until the production service publishes its final log-minimisation, retention, and deletion periods.

Backups exclude imported archives, downloads, extension packages, cookies, credentials, signing secrets, and caches. Credentials and extension trust records use Keychain and are not restored from backup.

Users can pause and reset local statistics and source reliability independently, remove downloads and Moments, disconnect MangaBaka, or delete the app to remove its application container.

A final privacy contact and effective date will be added before this draft becomes effective.

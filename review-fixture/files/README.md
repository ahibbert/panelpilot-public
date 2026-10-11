# Original CBZ import fixture

`panel-pilot-sample.cbz` is a deterministic comic archive for Panel Pilot's document-import and App Review path. It contains only:

- `001.png`, the CC0 original artwork documented in [`../ARTWORK.md`](../ARTWORK.md); and
- `ComicInfo.xml`, the metadata file published beside this README.

The archive is deliberately small and unencrypted. It is suitable for demonstrating import, natural page order, `ComicInfo.xml` parsing, right-to-left manga classification, offline reading, and on-device panel navigation. It contains no extension, script, credential, remote URL, or executable content.

Download URL:

`https://raw.githubusercontent.com/ahibbert/panelpilot-public/main/review-fixture/files/panel-pilot-sample.cbz`

Rebuild rules:

- archive entries are ordered `001.png`, then `ComicInfo.xml`;
- both entries use the ZIP epoch timestamp `1980-01-01 00:00:00`;
- both entries use deflate compression and Unix mode `0644`;
- the artwork bytes must match SHA-256 `7ea14e5115075c0798f438c14b974b11b0581eb292c54172475471b9e2119578`.

The archive SHA-256 is recorded below after generation and must change if either input changes.

- CBZ SHA-256: `4c574fde19c0b78735bb032891e591f03dde38e4252854b475572bc55f92bfec`

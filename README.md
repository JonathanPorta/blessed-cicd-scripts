# blessed-cicd-scripts

Public, signed exports of selected [blessed-cicd](https://github.com/JonathanPorta/blessed-cicd) scripts.
This repository is pipeline-only: exports arrive as releases built, verified and signed in
blessed-cicd's private CI. Nothing here is edited by hand.

Each release (`<export>-v<version>`) carries the export tarball, `MANIFEST.sha256`,
`MANIFEST.sha256.sig` and `SOURCE.json`. Verify `MANIFEST.sha256.sig` with the ed25519 key
`blessed-cicd-script-export-2026-10`, pinned from a copy of `.github/export-trust-store.json`
you confirmed with the owner out of band, before trusting anything else in a release.
The exported files carry their own licence (`LICENSE` inside each export); this repository's
other files are not licensed for reuse.

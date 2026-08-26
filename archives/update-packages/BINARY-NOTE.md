# Binary package storage note

The reserve path is created and integrity metadata is recorded. Historical ZIPs are the source-of-truth package artifacts; their SHA-256 values are in `MANIFEST.md`.

For large package binaries, preserve the original ZIP byte-for-byte. Do not rebuild an archive and assume it is identical unless its SHA-256 matches the manifest.

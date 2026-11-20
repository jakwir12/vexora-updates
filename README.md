# VEXORA AI-CARES CIT: update feed

Signed release manifests for VEXORA AI-CARES CIT installations, served with GitHub Pages:

- `stable.json`: production releases
- `beta.json`: release candidates (`-rc`), for lab nodes

Nodes set `VEXORA_UPDATE_FEED_URL=https://jakwir12.github.io/vexora-updates`.

This repository holds only signed manifests (version, notes, image references and their
Ed25519 signature). No code, no secrets. Files are written by the release workflow of the
main repository; do not edit them by hand. A node refuses any entry whose signature does not
match the Clarus-IT release key built into its image, so tampering here cannot install anything.

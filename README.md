# syn-scan

Scan files at rest for malware, and put what turns up aside

## Install

```bash
curl -sL https://soslinux.org/synapseos-update-key.asc | gpg --import   # once
git clone https://github.com/velle999/syn-scan
cd syn-scan && makepkg -si
```

makepkg fetches the source for this PKGBUILD's exact version from this
repository's releases, so a clone can only ever build the source it was
written against. `.SRCINFO` lists what it needs.

The source is signed with the SynapseOS update key, and makepkg refuses it
unless the signature is good. The fingerprint is in
[SECURITY.md](https://github.com/velle999/SYNAPSE/blob/main/SECURITY.md).

## Where this comes from

Developed in [the SynapseOS monorepo](https://github.com/velle999/SYNAPSE),
in `syn-scan/`. **This repository is generated from it** — the PKGBUILD, a
generated `.SRCINFO` and this README — so issues and patches belong there.

syn-scan 0.1.0-6 · GPL-2.0-or-later

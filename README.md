# G-SEND.IO releases

Download and update host for **G-SEND.IO** — the CNC G-code editor and
shop toolkit by [3D Distributed](https://3ddistributed.com).

This repository carries **release artifacts only** — no source code:

- [`version.json`](version.json) — the update manifest the app checks
  (weekly, on a background thread).
- **Releases** (right sidebar) — the signed Windows installers,
  `G-SEND.IO-Setup-<version>.exe`.

## Installing

Download the latest `G-SEND.IO-Setup-<version>.exe` from
[Releases](../../releases/latest), run it, and click **Install**. The app
installs to `C:\G-SEND` and appears in your Start Menu. Installed copies
find future updates by themselves and install them when you close the app.

## Integrity

Every installer is Authenticode-signed (Microsoft Azure Trusted Signing,
publisher *shane hooper*). The app's built-in updater additionally
verifies the SHA-256 in `version.json` and refuses any download whose
signature Windows will not vouch for. If you download manually, check the
digital signature in the file's **Properties → Digital Signatures** tab.

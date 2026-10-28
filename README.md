# Pi Extension Portable

Portable distributions for Pi extensions. Each extension is kept as a separate versioned directory and release asset.

## Available extensions

### `@koltmcbride/pi-loop` v0.4.1

- Package directory: `pi-loop-portable-extension-v0.4.1/`
- Archive: `pi-loop-portable-v0.4.1.tar.gz`
- Checksum: `pi-loop-portable-v0.4.1.SHA256SUMS`
- Release: [v0.4.1](https://github.com/movitecc/pi_extension_portable/releases/tag/v0.4.1)

### `pi-hermes-memory` v0.9.11

- Package directory: `pi-hermes-memory-portable-extension-v0.9.11/`
- Archive: `pi-hermes-memory-portable-v0.9.11.tar.gz`
- Checksum: `pi-hermes-memory-portable-v0.9.11.SHA256SUMS`
- Upstream: [chandra447/pi-hermes-memory](https://github.com/chandra447/pi-hermes-memory) at `bb58c12e853a52a4b92b10ff43c0394bca3f17ff`

Includes production npm dependencies and the Linux x86_64 Node 22 native SQLite addon. See `README-portable.md` for compatibility details. Install locally with `pi install ./pi-hermes-memory-portable-extension-v0.9.11 --no-approve`.

Release: [v0.9.11](https://github.com/movitecc/pi_extension_portable/releases/tag/v0.9.11)

This repository stores only extension portable packages. Pi, Node.js, credentials, sessions, and host configuration are not bundled.

Install an extension on a machine with compatible Pi:

```bash
tar -xzf pi-loop-portable-v0.4.1.tar.gz
pi install ./pi-loop-portable-extension-v0.4.1 --no-approve
pi list
```

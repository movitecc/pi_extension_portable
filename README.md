# Pi Extension Portable

Portable distributions for Pi extensions. Each extension is kept as a separate versioned directory and release asset.

## Available extensions

### `@koltmcbride/pi-loop` v0.4.1

- Package directory: `pi-loop-portable-extension-v0.4.1/`
- Archive: `pi-loop-portable-v0.4.1.tar.gz`
- Checksum: `pi-loop-portable-v0.4.1.SHA256SUMS`
- Release: [v0.4.1](https://github.com/movitecc/pi_extension_portable/releases/tag/v0.4.1)

This repository stores only extension portable packages. Pi, Node.js, credentials, sessions, and host configuration are not bundled.

Install an extension on a machine with compatible Pi:

```bash
tar -xzf pi-loop-portable-v0.4.1.tar.gz
pi install ./pi-loop-portable-extension-v0.4.1 --no-approve
pi list
```

# pi-hermes-memory portable package

This is the upstream `pi-hermes-memory` v0.9.11 extension packaged for local/offline distribution. Upstream source and version are recorded in `UPSTREAM.json`.

## Requirements

- Pi Coding Agent >= 0.80.6
- Linux x86_64 with Node.js 22.x (the bundled `better-sqlite3` native addon targets Node module ABI 127). Other Node versions, architectures, libc variants, and Bun need a matching rebuild/package.
- This package includes its production npm dependencies and native SQLite module. The remote machine does not need npm network access to load them when installed as a local package.

## Install

Extract the archive and install from its local folder:

```sh
tar -xzf pi-hermes-memory-portable-v0.9.11.tar.gz
pi install ./pi-hermes-memory-portable-v0.9.11 --no-approve
pi list
```

If Pi prompts to install dependencies or changes package contents, run the provided `npm ci --offline --omit=dev` inside the extracted package first; then start Pi with the same Node 22 runtime. A remote with no npm cache must use the already bundled `node_modules`.

The package includes no Pi executable, Node runtime, credentials, sessions, or personal memory.

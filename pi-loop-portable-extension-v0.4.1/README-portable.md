# pi-loop portable plugin

This archive contains only the Pi extension `@koltmcbride/pi-loop` v0.4.1.
It does not include Pi, Node.js, model credentials, sessions, or personal state.

## Install into Pi

From the extracted directory:

```bash
pi install ./pi-loop-portable-v0.4.1 --no-approve
pi list
```

The package manifest declares `./loop.ts` as the extension entrypoint.
Pi supplies the peer APIs (`@earendil-works/pi-coding-agent`,
`@earendil-works/pi-tui`, and `typebox`).

## Portable/offline use

Copy this directory to another machine with a compatible Pi installation and
install it from the local path. To keep loop state isolated from the host,
start Pi with a bundle-local directory, for example:

```bash
PI_CODING_AGENT_DIR=/path/to/pi-home pi
```

The extension itself has no runtime npm dependencies and contains no secrets.
The loop still needs Pi's configured model/provider when it fires.

## Commands

```text
/loop 15m <prompt>
/loop list
/loop stop
```

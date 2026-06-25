# CLAUDE.md — meme-me-cli

## What this is

Popup GIF meme overlay CLI — display a meme anywhere on screen with configurable
position, duration, audio, and animation. Package description, verbatim: "Popup gif
meme on any place on screen. Highly professional, highly stupid."

Part of the **MeMeMe-LLP** org. Repo is **private** (see workspace `CLAUDE.md` →
senzhang-* / org visibility rules; MeMeMe-LLP repos are private).

## Status

**Early-stage scaffold.** The overlay rendering (electron/webview) is still TODO.
`bin/meme.js` is the CLI entry point but core functionality is not wired yet.
Don't assume a feature exists — read `bin/meme.js` before claiming behavior.

## Tech stack

- Node.js, vanilla JavaScript — **no framework, no runtime deps** by design.
- Entry point: `bin/meme.js`, exposed as the `meme` binary via the `bin` field in
  `package.json`.

## Layout

```
bin/meme.js     # CLI entry point (scaffold)
package.json    # metadata + bin symlink
```

## Commands

- No build step.
- `npm test` — currently unimplemented (placeholder).
- Run the CLI via the `meme` symlink once linked, or `node bin/meme.js`.

## Working here

- It's a toy/scaffold — keep dependencies at zero unless the overlay work
  genuinely needs them; flag any dep addition explicitly.
- No README yet; this file is the orientation doc until one exists.

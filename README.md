# snap-dsf

**diff-so-fancy as a [Snap](https://snapcraft.io) package.**

[diff-so-fancy](https://github.com/so-fancy/diff-so-fancy) makes your diffs human-readable instead of machine-readable — better code review quality, faster defect spotting. This repo packages it as a strictly-confined Snap, making it a single-command install on any Linux distribution that supports snaps.

## Install

[![Get it from the Snap Store](https://snapcraft.io/en/dark/install.svg)](https://snapcraft.io/diff-so-fancy)

```bash
sudo snap install diff-so-fancy
```

## Usage

Pipe `git diff` through it:

```bash
git diff | diff-so-fancy
```

Or set it as your default Git pager/diff highlighter — see the [upstream docs](https://github.com/so-fancy/diff-so-fancy#usage) for configuration examples.

## How it works

The Snap wraps a pinned release of diff-so-fancy (tracked by Renovate and built with Perl's `fatpack`). A CI workflow verifies every push and PR still builds, while [snapcraft.io](https://snapcraft.io) handles publishing to the Snap Store on its own schedule.

## Disclaimer

This is a **community-maintained Snap**, not an official so-fancy project. The upstream maintainers have [approved](https://github.com/so-fancy/diff-so-fancy/pull/434) this packaging effort, but issues with the Snap itself should be reported here rather than upstream.

## Credits

- **[so-fancy/diff-so-fancy](https://github.com/so-fancy/diff-so-fancy)** — the excellent diff formatter this Snap packages.
- **[barryprice](https://github.com/barryprice)** — Snap packaging and maintenance.

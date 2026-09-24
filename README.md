# gentoo-tronbrowser

Gentoo overlay for [TronBrowser](https://tronbrowser.dev), an open-source,
privacy-first, AI-native browser built on Ungoogled Chromium.

## Install

```sh
eselect repository add tronbrowser git https://github.com/profullstack/gentoo-tronbrowser.git
emaint sync -r tronbrowser
emerge -av net-misc/tronbrowser-bin
```

This is the binary package: it installs the TronBrowser launcher and its bundled
extensions, and drives `www-client/chromium`, which portage pulls in as a runtime
dependency. `tron` and `tronbrowser` both land in `/usr/bin`.

## Updating

Ebuilds here are generated from `distribution/gentoo/` in
[profullstack/tronbrowser.dev](https://github.com/profullstack/tronbrowser.dev)
on each release.

# GooberNet Browser stage app

Static Scramjet browser application for embedding inside the TurboWarp stage through the companion unsandboxed extension.

Publish this entire directory on an HTTPS static host. The companion extension's default URL is:

`https://siegma2.github.io/goobernet/navigator-stage/`

This app registers its service worker at its own origin and uses Scramjet + BareMux + Libcurl/Wisp for live website browsing. Do not replace this with an iframe whose `src` is the destination website.

See the top-level `README.md` in the companion ZIP for setup steps and licensing information.

# GooberNet Browser stage app

Static Scramjet browser application for embedding inside the TurboWarp stage through the companion unsandboxed extension.

Publish this entire directory on an HTTPS static host. The companion extension's default URL is:

`https://waffleings.github.io/mewhenthe/`

This app registers its service worker at its own origin and uses Scramjet + BareMux + Libcurl/Wisp for live website browsing. Do not replace this with an iframe whose `src` is the destination website.

See the top-level `README.md` in the companion ZIP for setup steps and licensing information.


## TurboWarp display-only mode

The GooberNet extension supports two ways to use the stage browser:

- `navigate browser to [URL]` opens a page in the normal browser UI, where users can browse normally.
- `display website [URL]` opens the page with GooberNet's header, tabs, address bar, bookmarks, and browser status hidden so the website fills the stage.
- `show browser controls` returns to the normal browser UI without closing the current page.

Display-only mode hides GooberNet's own browser controls. The displayed website remains interactive, so links and navigation built into that website may still move to other pages. This mode is intended for presentation/embedded viewing, not as a security boundary against a determined user.

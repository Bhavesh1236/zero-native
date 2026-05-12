# Browser Example

A no-build vanilla HTML/CSS/JS example that uses the main WebView for browser chrome and a native overlay WebView for page content.

Run it from this directory:

```sh
zig build run
```

The frontend lives in `frontend/` and is served directly as `zero://app/index.html`.

The page content runs in an isolated native overlay WebView. Overlay pages do not receive `window.zero`; all navigation and sizing is controlled by the browser chrome through the overlay handle returned by `window.zero.webviews.create()`.

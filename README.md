# Louie: Zone 2 Run Buddy

The public site for Louie: a home page and the [privacy policy](https://thoughtandtheory.github.io/louie-app/privacy/).
The app itself lives in a private repo; the privacy page is copied from its `docs/privacy/index.html`.

The home page follows the Louie brand (tokens, Outfit type and Louie's art from the app repo's
`design/brand/louie/`), light and dark with the system. `assets/` holds the Outfit fonts (SIL OFL,
licence included) and the app icons; Louie's SVG is inlined so dark mode can recolour him.

The link-preview image is `assets/og-image.png` (1200×630). Its source is `tools/og-card.html`, which reuses the hero art and copy. To rebuild the image after changing the hero, open that file in Chrome at 1200×630, or run:

    "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --hide-scrollbars --force-device-scale-factor=1 --window-size=1200,630 --allow-file-access-from-files --screenshot=assets/og-image.png "file://$PWD/tools/og-card.html"

The Open Graph and Twitter tags use absolute URLs because link previews ignore relative ones.

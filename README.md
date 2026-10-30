# Baihaqi Studio: studio site

The home page of Baihaqi Studio at https://fighterloo.github.io/ (GitHub user site of FighterloO). Static: no build step.
GitHub Pages serves `main` from the root.

```
index.html        the page (all text lives here), with WebSite + Organization JSON-LD; the header's two swords are
                  the game's studio splash (src/game/transitions.js + src/styles/boot.css in the game repo)
404.html          not-found page (noindex)
css/site.css      styles: the game site's palette (dark navy, gold, bronze) and font
media/moonhaven-loop.mp4   header video: Moonhaven at night, leaves drifting (the game site's media/hero-loop.mp4, H.264 yuv420p)
img/moonhaven.webp         its poster, also shown for reduced motion
img/banner.webp   background under the header: the YouTube banner without its text (preview/youtube/raw/yt-banner-3d.png)
img/game-art.webp, img/game-logo.webp   the Legacy of Warden card (game site img/bg/release.webp, img/art/title-logo.webp)
img/share.jpg     1200x630 share image, made from the banner
favicon.ico, favicon-48x48.png   the Assassin's head (legacy of warden preview/youtube/the assassin.png, cropped)
favicon-192x192.png, apple-touch-icon.png, img/logo.png   the whole Assassin picture (logo.png = Organization logo)
sitemap.xml, robots.txt
```

The game has its own site: https://fighterloo.github.io/legacy-of-warden-site/ (repo FighterloO/legacy-of-warden-site),
which holds the Privacy Policy and Terms of Use.

Preview locally: `python -m http.server 8766`, then open http://localhost:8766/.
After changing `css/site.css`, bump the `?v=` number on its link in `index.html` and `404.html`.
A new game = a new `<li>` in `.games` in `index.html`.
When Google Play goes live, change the "Coming soon to Google Play" chip in `index.html`.

## Search Console

`google4adee214d00288e8.html` at the root verifies the Search Console property for https://fighterloo.github.io/. Never delete it.

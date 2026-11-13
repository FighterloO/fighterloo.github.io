# Baihaqi Studio: studio site

The home page of Baihaqi Studio at https://fighterloo.github.io/ (GitHub user site of FighterloO). Static: no build step.
GitHub Pages serves `main` from the root.

```
index.html        the page (all text lives here), with WebSite + Organization JSON-LD; the header's two swords are
                  the game's studio splash (src/game/transitions.js + src/styles/boot.css in the game repo)
404.html          not-found page (noindex)
css/site.css      styles: the game site's palette (dark navy, gold, bronze) and font
media/moonhaven-loop.mp4   Moonhaven at night, leaves drifting (the game site's media/hero-loop.mp4, H.264 yuv420p): the Legacy of Warden card's background
img/moonhaven.webp         its poster
img/head-*.webp            the header: the studio's worlds take turns behind the splash (warden-1/2: the game site's img/bg/features, planes; tower-1/2: Next Tower's town and a desert battle)
img/banner.webp   background under the header: the YouTube banner without its text (preview/youtube/raw/yt-banner-3d.png)
img/game-logo.webp         the Legacy of Warden card's logo (game site img/art/title-logo.webp)
media/nexttower-loop.mp4   the Next Tower card's background. Both card videos play only while on screen and rest during a scroll: the
                           inline script at the end of index.html; two videos decoding while scrolling made the page stutter. The clip: 10 s of reactions (Scalding Steam, Conduction, Frost Wall,
                           Plasma Burst) cut from the English trailer at 18.25 s, 960x540 24 fps H.264 CRF 28, muted (14 Nov 2026)
img/nexttower-poster.webp  its poster (the first frame)
img/nt-logo.webp           the Next Tower card's title in Silkscreen, transparent, subtitle cropped off (13 Nov 2026)
img/share.jpg     1200x630 share image, made from the banner
favicon.ico, favicon-48x48/96x96/192x192.png, apple-touch-icon.png, icon-512.png, img/logo.png
                  the studio mark: two crossed pixel swords on navy in a gold frame, drawn on a 24x24 grid and
                  scaled x2/x4/x8 nearest (user pick, 13 Nov 2026); logo.png = Organization logo; site.webmanifest
sitemap.xml       the studio page plus the game sites' pages (same host); robots.txt points to it and to each game
                  site's own sitemap. Google shows one favicon per host in Search, so this icon is the one search
                  results use for the game sites too.
```

The game has its own site: https://fighterloo.github.io/legacy-of-warden-site/ (repo FighterloO/legacy-of-warden-site),
which holds the Privacy Policy and Terms of Use.
Next Tower has its own site too: https://fighterloo.github.io/next-tower-site/ (repo FighterloO/next-tower-site), with its Privacy Policy.

Preview locally: `python -m http.server 8766`, then open http://localhost:8766/.
After changing `css/site.css`, bump the `?v=` number on its link in `index.html` and `404.html`.
A new game = a new `<li>` in `.games` in `index.html`.
When Google Play goes live, change the "Coming soon to Google Play" chip in `index.html`.

## Search Console

`google4adee214d00288e8.html` at the root verifies the Search Console property for https://fighterloo.github.io/. Never delete it.

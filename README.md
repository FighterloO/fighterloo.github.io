# Baihaqi Studio: studio site

The home page of Baihaqi Studio at https://fighterloo.github.io/ (GitHub user site of FighterloO). Static: no build step.
GitHub Pages serves `main` from the root.

```
index.html        the page (all text lives here), with WebSite + Organization JSON-LD
404.html          not-found page (noindex)
css/site.css      styles: the game site's palette (dark navy, gold, bronze) and font
img/banner.webp   the YouTube channel banner without its text (legacy of warden preview/youtube/raw/yt-banner-3d.png)
img/              game tile art copied from legacy-of-warden-site (Moonhaven, logo); share.jpg (1200x630) made from the banner
favicon.ico, favicon-48x48.png, favicon-192x192.png, apple-touch-icon.png   the game's icon
sitemap.xml, robots.txt
```

The game has its own site: https://fighterloo.github.io/legacy-of-warden-site/ (repo FighterloO/legacy-of-warden-site),
which holds the Privacy Policy and Terms of Use.

Preview locally: `python -m http.server 8766`, then open http://localhost:8766/.
After changing `css/site.css`, bump the `?v=` number on its link in `index.html` and `404.html`.
A new game = a new `<li>` in `.games` in `index.html`.
When Google Play goes live, change the "Coming soon to Google Play" chip in `index.html`.

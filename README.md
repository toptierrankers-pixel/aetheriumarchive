# The Aetherium Archive

An unofficial Elder Scrolls fan site: lore, series history, and a TES VI watch page.

## What's in here

```
index.html        Home
lore.html          Lore of Tamriel
history.html       Series timeline, Arena (1994) → Blades
tes6.html          TES VI: confirmed facts vs. fan speculation
css/style.css      All styling (design tokens at the top of the file)
js/main.js         Mobile nav toggle
favicon.svg        Favicon (modern browsers)
favicon.ico        Favicon fallback (16/32/48px, older browsers)
assets/logo.svg    Full logo mark, used in the header and hero
assets/apple-touch-icon.png   180×180 icon for iOS home screens
assets/icon-*.png  Extra rendered sizes of the logo, in case you need them elsewhere
```

No build step, no dependencies to install, it's plain HTML/CSS/JS. Google Fonts (Cinzel, Crimson Text, JetBrains Mono) load from a CDN link in `style.css`.

## Deploy it

**Netlify / Vercel (drag-and-drop):** zip this folder (or the unzipped folder) and drop it on Netlify Drop (app.netlify.com/drop) or Vercel's dashboard. Nothing to configure.

**GitHub Pages:** push this folder's contents to a repo, then in the repo's Settings → Pages, set the source to the branch/root. Your site will be live at `https://<username>.github.io/<repo>/`.

**Any static host (S3, Cloudflare Pages, your own server):** upload the contents of this folder as-is to the web root. `index.html` is the homepage.

## Rebranding it later

- Colors, fonts, and spacing all live at the top of `css/style.css` under `:root`, change the hex values there and the whole site updates.
- The site name ("The Aetherium Archive") appears in the `<title>`, the header `.brand-name`, and the footer of each page, search and replace if you rename it.
- The logo is one SVG (`assets/logo.svg`) reused everywhere, so redrawing that one file updates the header, hero, favicon, and touch icon source.

## Content note

Lore and history pages summarize widely known, publicly available facts about the Elder Scrolls series in original wording, no game text is reproduced. The site includes a fan/non-affiliation disclaimer in the footer of every page; keep that if you publish this.

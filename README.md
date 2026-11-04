# kevindemo.github.io

Source of Kevin Chen's freelance homepage, served by GitHub Pages at https://kevindemo.github.io.

Plain HTML and CSS with no build step, no framework, no JavaScript, and no analytics or trackers. The only external requests are Google Fonts. Light and dark modes follow the visitor's system setting.

Two design directions are in this repo until one is picked. `index.html` with `styles.css` is Direction A (Waybill). `design-b/index.html` is Direction B (Almanac), self-contained and set to `noindex`. Delete the one that is not chosen; if B wins, move it to the root and remove its `noindex` line.

To preview it, open `index.html` in a browser, or run `python -m http.server` in this folder.

The CV at `/cv/` is served from a separate repository. This site only links to it, and because this repo has no `cv` folder the two do not conflict.

The result figures on the page come from the READMEs of the demo repositories. Update them here if those results change. Each unfinished demo has a `RESULT PLACEHOLDER` comment where its real result line goes.

When the Upwork profile exists, add its link at the placeholder comment in the Contact section.

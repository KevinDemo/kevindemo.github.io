# kevindemo.github.io

Source of Kevin Chen's freelance homepage, served by GitHub Pages at https://oct28th.com.

Plain HTML and CSS with no build step, no framework, and no analytics or trackers. The only external requests are Google Fonts. Two small inline scripts handle the theme switcher (System, Light, Dark) and the measurement bars; without JavaScript the page still works and follows the visitor's system setting.

The visual system is documented in `DESIGN.md`.

To preview it, open `index.html` in a browser, or run `python -m http.server` in this folder.

The CV at `/cv/` is served from a separate repository. This site only links to it, and because this repo has no `cv` folder the two do not conflict.

The result figures on the page come from the READMEs of the demo repositories. Update them here if those results change. Each unfinished demo has a `RESULT PLACEHOLDER` comment where its real result line goes.

When the Upwork profile exists, add its link at the placeholder comment in the Contact section.

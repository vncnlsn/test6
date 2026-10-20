# APS Land Services - Concept V6: Precision / Dark

A clean-slate, dark-first, three-color static website concept. No framework or build step.

## Preview
Run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Design tokens
- Deep charcoal navy: `#101820`
- Soft mineral white: `#e6e8e5`
- Muted steel blue: `#879dad`

Transparency and CSS gradients use only these three base colors. Photography is monochrome.

## Architecture
- Four HTML pages
- `css/site.css`: single shared stylesheet
- `js/site.js`: mobile navigation, email-handoff form, marquee
- `js/us-map.js`: original unchanged geographic map code
- `assets/`: supplied original assets

## Notes
- The contact form uses `mailto:` and does not send or store submissions. It depends on the visitor having an email application configured.
- Marquee external destinations are inherited from the prior concept and require final owner review; historical names may have changed.
- The interactive map contains the original coverage data and state interactions.
- Metadata, canonical URLs, JSON-LD, sitemap and robots assume deployment at `https://apsland.com/`. Verify Cloudflare clean-URL routing and redirects before publishing.
- Design prototype: perform responsive browser QA, accessibility audit and form tests before production.

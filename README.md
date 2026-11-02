# Taco Bell Cyclospora Lawsuit Landing Page — GitHub Pages (static) version

A static (HTML + CSS only, no PHP) landing page for the **Taco Bell Cyclospora outbreak claims** sponsored by **Andrews & Higgins**, built on the framework of your uploaded birthing-injury page (`index-6.html` / `style-6.css` — including your parallax hero and commented-out header) and filled with content from **tacobelllawsuithelp.com**. Per your standing instruction, all branding and firm-information areas were converted to the sample site's firm.

## Kept from your framework, unchanged

- Page structure, classes, the MTAA CIPA block script, and your Meta Pixel (`1665132690448359`).
- Your form embed: `forms.mtaa.ai/f/nf_441462e043274be8bab32ea3e44ac34c`, in the overflow form card — the container hangs past the hero over the section below it, the frame scrolls internally with `overflow: auto` if the embed runs tall, and your mobile values from the framework are preserved.
- The commented-out site header block (converted inside the comment to the new firm, so it is correct if you uncomment it), with the firm name carried in the hero, as in your framework.
- The call/text consent paragraph in the footer disclaimer.
- Footer legal links still point to your `privacy-policy.html` and `disclaimer.html` on justicehelpnow.com (your hosted legal pages from the framework).

## Parallax hero — retained as a placeholder, two notes

- Your `.section-parallax` block is retained in the CSS and the hero keeps the `section-parallax` class. The overlay tint was recolored with the rest of the palette to the sample's hero navy (`--overlay-rgb: 9, 29, 68`, opacity still 0.75).
- **Image URL:** the framework's URL pointed to a birth-injury photo (`mom-baby2.jpg`), so that one line now reads `url("YOUR-IMAGE-URL-HERE")` as the placeholder. Send the new image URL and it drops into that same line — or swap it yourself in `css/style.css` (search for `YOUR-IMAGE-URL-HERE`). Until then the hero renders as the navy overlay color over the hero gradient.
- **One-word fix inside your block:** the mobile fallback targeted `.section--parallax` (double hyphen) while the class is `.section-parallax`, so the iOS `background-attachment: scroll` fallback could never apply. It now targets `.section-parallax`. Nothing else in the block was restructured.

## Firm information — converted to the sample site (Andrews & Higgins)

- Title/meta, hero firm line, and team block: Andrews & Higgins; the attorney featured on the sample page, **Anne Andrews**, replaces the prior founder block (her photo lives on the sample's CDN and was not hotlinked).
- Footer contact: Andrews & Higgins, 4701 Von Karman Ave, Newport Beach, CA 92660.
- Disclaimer: the sample's sponsorship line — "THIS IS ATTORNEY ADVERTISING sponsored by Andrews & Higgins, located at 4701 Von Karman Ave, Newport Beach, CA 92660" — plus the sample's "No representation is made that the quality of the legal services to be performed is greater than the quality of legal services performed by other lawyers. Co-counsel associated."
- Copyright: © 2026 Andrews & Higgins.
- **No phone number:** none is displayed anywhere on the sample site (checked in both the page text and a live rendered inspection), and the framework is the phoneless variant, so the page has no phone.
- All prior-firm traces verified at zero: no Lerner and Rowe names, numbers, addresses, or image hosts (familyjusticenow.com is gone from both files, including inside the commented header), and no birth-injury content anywhere.

## Colors and typeface

`css/style.css` is your uploaded `style-6.css` with **color and font-family values only** changed (diff-verified — every layout, spacing, and overflow rule untouched), matched to the live tacobelllawsuithelp.com design, sampled from the rendered site on 2026-11-02:

- Dark navy `#0c1f3d` (their footer) for the top bar, dark section, and footer; royal blue `#0a3984` (their top logo bar) through the hero gradient to hero navy `#091d44`
- Medium blue `#1e57a3` for kickers, headline accents, and checkmark circles (white checks, as on the sample), with sky blue `#6cd9ff` for highlights on dark backgrounds (hero eyebrow, dark-section kicker, footer heading accents)
- Bright green `#22a717` CTA buttons with white text, like their "DO I QUALIFY?" button (hover `#1e9413`)
- Light gray-blue `#d5d9e2` (their form-panel tone) for the fee band and border lines
- **Typeface:** their headlines are a heavy, rounded sans-serif (Arial/Helvetica-like; no exact family is identifiable from the rendered page) and their body text is a regular sans, so the framework's serif display font (Fraunces) was replaced in all four heading declarations by Inter — the framework's own sans, already loaded — with Arial/Helvetica fallbacks, and the Google Fonts link no longer loads Fraunces. Weights and sizes are unchanged.
- The sample also uses a pure-red accent (`#ff0000`) for its "Pre-Qualify Now" label and footnote; the framework has no equivalent element, so red was not mapped. Colors were sampled visually from the rendered page, so they are close approximations rather than values read from that site's stylesheet.

## Content (from tacobelllawsuithelp.com)

- Hero: their headline — "Sick After Eating Taco Bell? You May Be Entitled to Compensation" — with their summary: the CDC is investigating a multistate Cyclospora outbreak linked to shredded iceberg lettuce served at certain Taco Bell locations; free consultation, no fee unless we win.
- What Happened — in July 2026 the CDC and FDA announced a Cyclospora outbreak investigation; shredded iceberg lettuce at Taco Bell locations in five states is the suspected source; investigators traced it to Taylor Farms in Mexico, which recalled all iceberg lettuce from its Central Mexico farm in the U.S. market; the CDC believes thousands have been affected and the number continues to rise.
- Were You Affected? — the Cyclospora/cyclosporiasis explainer and their five qualifiers: ate Taco Bell during the outbreak period; location in Indiana, Kentucky, Michigan, Ohio, or West Virginia (potentially other states); severe gastrointestinal illness afterward; tested positive for Cyclospora or received treatment consistent with cyclosporiasis; missed work or incurred medical expenses. Their note that completing the evaluation does not guarantee compensation is included.
- Inside the Cyclospora Outbreak — nine cards built from their announced facts (investigation, suspected source, five states, supplier, origin, recall, the parasite, the illness, the scale).
- No Fee Unless We Win — their terms: no upfront costs; a fee only if compensation is recovered. (The sample publishes no results figure, so none was invented for this band.)
- What We Look At — their form's details: what/when you ate, the state, the illness, treatment (doctor visit or hospital stay — none, less than a day, 1, 2, or over 2 nights), diagnosis/testing status, and missed work/medical expenses.

## Files

```
github-taco-bell-lawsuit-landing-page/
├── index.html
├── css/style.css   (your framework CSS, colors + font only changed)
└── README.md
```

Publish the same way as the other GitHub pages: upload to a repo keeping the structure, Settings → Pages → deploy from branch (root).

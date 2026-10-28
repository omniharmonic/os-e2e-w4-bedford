# Import report: Bedford

Imported from https://bedford-demo.squarespace.com (Squarespace 7.0) on 2026-10-28 with `openspace import squarespace`.
Sources: page HTML and the sitemap, Squarespace's `?format=json` data (owner mode). 125 requests.

## Summary

- **8** pages, **3** collection items in 1 collection(s)
- **27** media files (3.4 MB) downloaded into `media/`
- **4** redirects so old addresses keep working
- **4** item(s) need your attention (below)

## Pages

| Squarespace | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Home | 5 | 10 |
| `/what-we-do-bedford` | `/what-we-do-bedford` | What We Do | 5 | 9 |
| `/projects-bedford` | `/projects-bedford` | Projects | 2 | 8 |
| `/partners-bedford` | `/partners-bedford` | Partners | 4 | 8 |
| `/contact-bedford` | `/contact-bedford` | Contact | 2 | 4 |
| `/read-me-bedford` | `/read-me-bedford` | Read Me | 32 | 61 |
| `/take-action-bedford` | `/take-action-bedford` | Take Action | 3 | 7 |
| `/home-alt-bedford` | `/home-alt-bedford` | Home Alt | 1 | 2 |

## Collections

| Squarespace | OpenSpace | Kind | Items | Drafts |
| --- | --- | --- | ---: | ---: |
| `/news-bedford` | `/news-bedford/` | blog | 3 | 0 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying Squarespace's template CSS or code.

- Brand color #36b3a8 (Squarespace "accent" color).
- Fonts on Squarespace: adobe-garamond-pro → pairing "Fraunces & Hanken Grotesk" (Fraunces / Hanken Grotesk), the closest curated match. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on Squarespace: Heading 1 is 1.8× body text. Density "airy" from the section heights.
- adobe-garamond-pro (licensed from Adobe Fonts) can't be copied, so EB Garamond — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- proxima-nova (licensed from Adobe Fonts) can't be copied, so Sofia Sans — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Type scale on Squarespace (the live site, measured in a browser) kept: display 68px caps, heading 1 32px/30px, body 18px/18px.
- Page rhythm on Squarespace (the live site, measured in a browser): sections padded 59px (22px on phones) — kept in Site Styles.
- The contrast solver adjusted 3 color pairing(s) so every section theme meets WCAG AA (e.g. light accent, light accent-hover).

Design check: 0 error(s), 21 warning(s).

- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/what-we-do-bedford): “What We Do” has no clear call to action — nothing tells visitors what to do next.
- warning (/what-we-do-bedford): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/projects-bedford): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/projects-bedford): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/projects-bedford): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/projects-bedford): This block still has placeholder text (“Lorem ipsum”).
- warning (/projects-bedford): “Projects” has no clear call to action — nothing tells visitors what to do next.
- warning (/partners-bedford): This block still has placeholder text (“Lorem ipsum”).
- warning (/partners-bedford): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- … and 9 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Custom code and embeds

- Site-wide Code Injection was found (1 snippet(s)). It was **not** copied: review it and add what you still need in Settings → Advanced (head/footer code). Squarespace-specific scripts won't work here. _(site)_

### Forms and newsletter

- Form "New Form" recreated with 4 field(s). Submissions now arrive in the OpenSpace inbox; Squarespace form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/partners-bedford)_
- Newsletter signup recreated. Squarespace Email Campaigns / Mailchimp subscribers are not moved: export your list from Squarespace and import it in the Hub. _(footer)_

### Links

- Navigation link "Sign In My Account" (#) leads to a page that wasn't imported; it was left out. _(navigation)_

### Design

- A photo section's overlay was darkened from 30% to 70% so its text stays readable. _(/, /read-me-bedford)_
- A photo section's overlay was darkened from 30% to 45% so its text stays readable. _(/what-we-do-bedford, /projects-bedford, /partners-bedford, /contact-bedford, +1 more)_

### Other

- The page had no Heading 1; its first heading was made the Heading 1 (search engines and screen readers use it). _(/contact-bedford)_

## Redirects

Saved in `content/site.json` (`redirects`), published with the site:

| From | To |
| --- | --- |
| `/news-bedford/2014/1/23/get-out-there` | `/news-bedford/get-out-there/` |
| `/news-bedford/2014/1/23/why-deserts-matter-too` | `/news-bedford/why-deserts-matter-too/` |
| `/news-bedford/2014/1/23/appalachia` | `/news-bedford/appalachia/` |
| `/landing-bedford` | `/` |

## Not moved by the importer

- Orders, customers, inventory, discounts, gift cards, shipping and tax settings (commerce stays in Squarespace until you switch).
- Newsletter subscribers, form submissions, member accounts and blog comments.
- Scheduling (Acuity), donations, digital-download files and anything behind a login.
- Squarespace analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:import-squarespace` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (Squarespace Domains or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the Squarespace subscription until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain away from Squarespace if you like).


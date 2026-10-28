# Visual fidelity

Overall match: **75/100** — fonts, type sizes, spacing and each section measured in a browser on both sites (75%), and how alike the pages look as pictures (25%). How it's scored: docs/qa/import-fidelity.md.

Auto-tuning raised it from 66/100:

- h2: 25px, 25px on phones
- h3: 16px, 16px on phones, tracking 0em
- h2: in the label font, as on the original
- h3: in the label font, as on the original
- section padding on phones 35px
- /contact-bedford: 1 section(s) at the narrow width, as on the original
- /partners-bedford: 3 section(s) at the narrow width, as on the original
- /projects-bedford: 1 section(s) at the narrow width, as on the original
- button corners sharp
- buttons on dark sections #36b3a8, as on the original
- buttons on light sections #27aa9f, as on the original
- /contact-bedford: section 1 507px tall, as on the original
- /partners-bedford: section 1 507px tall, as on the original
- /projects-bedford: section 1 507px tall, as on the original
- /: section 3 recreated as a custom component
- /: section 4 recreated as a custom component

Without custom components: 74/100; with the sections recreated as components: 75/100.

## / at 1440px — 80/100

Checks 81/100 · looks alike 78/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/landing-bedford/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Lead text size | 23px | 23px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 15px | 15px | same |
| Buttons letter spacing and case | 0.133em, uppercase | 0.133em, uppercase | same |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Section padding | 59px | 59px | same |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | We conserve land through outreach, restoration, and research. | 71 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Italic lines: 1 → 0; Height: 223px → 156px |
| 3 | (no heading) | 67 | Text: adobe-garamond-pro 23px → EB Garamond 23px; Text color: #000000 → #13130d; Columns: 3 → 2 |
| 4 | (no heading) | 67 | Text: adobe-garamond-pro 23px → EB Garamond 23px; Text color: #000000 → #13130d; Columns: 3 → 2 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Set the closing/pull line in italics (lead style).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## / at 390px — 74/100

Checks 74/100 · looks alike 74/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/landing-bedford/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 13px | 13.1px | same |
| Buttons letter spacing and case | 0.154em, uppercase | 0.133em, uppercase | same |
| Section padding | 21.5px | 51.5px | **differs** |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | We conserve land through outreach, restoration, and research. | 71 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Italic lines: 1 → 0; Height: 396px → 180px |
| 3 | (no heading) | 100 | — |
| 4 | (no heading) | 71 | Text: adobe-garamond-pro 17.2px → EB Garamond 18px; Text color: #000000 → #13130d; Height: 253px → 542px |
| 5 | (no heading) | 0 | Present:  → no matching section |
| 6 | (no heading) | 71 | Text: adobe-garamond-pro 17.2px → EB Garamond 18px; Text color: #000000 → #13130d; Height: 253px → 515px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPaddingMobile = 22
- Set the closing/pull line in italics (lead style).
- Bring this section across (or check it was merged into another).

## /contact-bedford at 1440px — 78/100

Checks 77/100 · looks alike 81/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/contact-bedford/  
Imported: /contact-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | adobe-garamond-pro | Sofia Sans | **differs** |
| Buttons size | 15px | 13px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0.154em, uppercase | **differs** |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Content width | 446px | 448px | same |
| Section padding | 96px | 15px | **differs** |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | CALL OR VISIT | 85 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Image placement: right, 25% wide → none |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.size = 15
- choices.typography.scale.button = { letterSpacing: 0, case: "uppercase" }
- choices.layout.sectionPadding = 96
- Adjust the stack column spans (image column) or the image's side.

## /contact-bedford at 390px — 62/100

Checks 58/100 · looks alike 74/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/contact-bedford/  
Imported: /contact-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | adobe-garamond-pro | Sofia Sans | **differs** |
| Buttons size | 15px | 13.1px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0.133em, uppercase | **differs** |
| Section padding | 42px | 9px | **differs** |
| Button corners | 0px | 9999px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | CALL OR VISIT | 46 | Heading: proxima-nova 25px → Sofia Sans 25px; Columns: 3 → 5; Image placement: right, 67% wide → none; Height: 506px → 855px |
| 3 | EMAIL | 64 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 1 → 5; Height: 444px → 855px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 15
- choices.typography.scale.button = { letterSpacing: 0, case: "uppercase" }
- choices.layout.sectionPaddingMobile = 42
- choices.shape = "sharp"
- Fewer columns: merge them into one stack column.
- Adjust the stack column spans (image column) or the image's side.

## /home-alt-bedford at 1440px — 69/100

Checks 74/100 · looks alike 53/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/home-alt-bedford/  
Imported: /home-alt-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 15px | 15px | same |
| Buttons letter spacing and case | 0.133em, uppercase | 0.133em, uppercase | same |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: A better world STARTS WITH A CHOICE CONT → no matching section |
| 2 | This page demonstrates how you can use the Page Slideshow functionality. | 67 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 1 → 4; Height: 85px → 1176px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).
- Fewer columns: merge them into one stack column.

## /home-alt-bedford at 390px — 59/100

Checks 61/100 · looks alike 55/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/home-alt-bedford/  
Imported: /home-alt-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 13px | 13.1px | same |
| Buttons letter spacing and case | 0.154em, uppercase | 0.133em, uppercase | same |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: A better world STARTS WITH A CHOICE CONT → no matching section |
| 2 | (no heading) | 40 | Columns: 1 → 4; Height: 108px → 545px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).
- Fewer columns: merge them into one stack column.

## /partners-bedford at 1440px — 83/100

Checks 81/100 · looks alike 88/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/partners-bedford/  
Imported: /partners-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 15px | **differs** |
| Buttons letter spacing and case | 0.167em, uppercase | 0.133em, uppercase | same |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Content width | 446px | 448px | same |
| Section padding | 96px | 73.5px | same |
| Button corners | 0px | 9999px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | Our partners are so important and we accomplish a lot together etc. Lorem ipsum dolor sit amet, cons | 53 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Columns: 4 → 1; Height: 1504px → 378px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.size = 18
- choices.shape = "sharp"
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /partners-bedford at 390px — 65/100

Checks 59/100 · looks alike 84/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/partners-bedford/  
Imported: /partners-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 13.1px | **differs** |
| Buttons letter spacing and case | 0.167em, uppercase | 0.133em, uppercase | same |
| Section padding | 39.5px | 46px | same |
| Button corners | 0px | 9999px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 33 | Columns: 1 → 2 |
| 2 | (no heading) | 100 | — |
| 3 | PARTNERS | 11 | Background: #ffffff → #13130d; Heading: proxima-nova 25px → Sofia Sans 44.1px; Columns: 2 → 1; Image placement: left, 44% wide → center, 100% wide; Image crop: 1:1 → 0.77:1 |
| 4 | BECOME A PARTNER | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 168px → 783px |
| 5 | (no heading) | 0 | Present: Name First Name (required) Last Name (re → no matching section |
| 6 | (no heading) | 80 | Height: 307px → 783px |
| 7 | (no heading) | 0 | Present: SUBMIT → no matching section |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 18
- choices.shape = "sharp"
- Fewer columns: merge them into one stack column.
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).
- Bring this section across (or check it was merged into another).

## /projects-bedford at 1440px — 76/100

Checks 76/100 · looks alike 74/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/projects-bedford/  
Imported: /projects-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | adobe-garamond-pro | Sofia Sans | **differs** |
| Buttons size | 15px | 13px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0.154em, uppercase | **differs** |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Content width | 446px | 448px | same |
| Section padding | 96px | 29.5px | **differs** |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | Here's just a small sampling of the natural treasures we've helped preserve over the years. | 78 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Image placement: right, 69% wide → center, 31% wide; Height: 2461px → 1705px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.size = 15
- choices.typography.scale.button = { letterSpacing: 0, case: "uppercase" }
- choices.layout.sectionPadding = 96
- Adjust the stack column spans (image column) or the image's side.

## /projects-bedford at 390px — 76/100

Checks 75/100 · looks alike 80/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/projects-bedford/  
Imported: /projects-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 2 size | 25px | 25px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | adobe-garamond-pro | Sofia Sans | **differs** |
| Buttons size | 15px | 13.1px | **differs** |
| Buttons letter spacing and case | 0em, uppercase | 0.133em, uppercase | **differs** |
| Section padding | 42px | 18px | **differs** |
| Button corners | 0px | 9999px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | Here's just a small sampling of the natural treasures we've helped preserve over the years. | 95 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Text: adobe-garamond-pro 18px → EB Garamond 18px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.typography.scale.button.sizeMobile = 15
- choices.typography.scale.button = { letterSpacing: 0, case: "uppercase" }
- choices.layout.sectionPaddingMobile = 42
- choices.shape = "sharp"

## /read-me-bedford at 1440px — 88/100

Checks 89/100 · looks alike 87/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/read-me-bedford/  
Imported: /read-me-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 2 size | 25px | 25px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 15px | 15px | same |
| Buttons letter spacing and case | 0.133em, uppercase | 0.133em, uppercase | same |
| Navigation size | 13px | 13px | same |
| Navigation letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Site title size | 13px | 13px | same |
| Site title letter spacing and case | 0.154em, uppercase | 0.154em, uppercase | same |
| Content width | 956px | 1280px | **differs** |
| Section padding | 66.5px | 59px | same |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | Template Features | 67 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Columns: 2 → 1 |
| 3 | BANNER AREA | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 4 | SIDEBAR | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 243px → 330px |
| 5 | INDEX | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 6 | Style Editor Options | 53 | Heading: adobe-garamond-pro 32px → EB Garamond 32px; Columns: 2 → 1; Height: 627px → 186px |
| 7 | SITE NAVIGATION | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 8 | BANNER SECTION | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 9 | MAIN CONTENT | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 10 | SIDEBAR | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 11 | PREFOOTER | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 120px → 176px |
| 12 | FOOTER | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 13 | BLOG | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 14 | GALLERY STYLES | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 15 | EVENT STYLES | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 16 | PRODUCT STYLES | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 17 | (no heading) | 86 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 63px → 176px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.contentWidth = 956
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /read-me-bedford at 390px — 86/100

Checks 88/100 · looks alike 82/100 (screenshots compared).

Original: https://bedford-demo.squarespace.com/read-me-bedford/  
Imported: /read-me-bedford (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 2 size | 25px | 25px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 13px | 13.1px | same |
| Buttons letter spacing and case | 0.154em, uppercase | 0.133em, uppercase | same |
| Section padding | 34.5px | 35.5px | same |
| Button corners | 300px | 9999px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 100 | — |
| 2 | Template Features | 81 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Height: 318px → 128px |
| 3 | BANNER AREA | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 4 | SIDEBAR | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 5 | INDEX | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 6 | Style Editor Options | 81 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Height: 925px → 128px |
| 7 | SITE NAVIGATION | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 8 | BANNER SECTION | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 440px → 751px |
| 9 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 266px → 751px |
| 10 | MAIN CONTENT | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 278px → 536px |
| 11 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 209px → 536px |
| 12 | SIDEBAR | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 307px → 522px |
| 13 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 196px → 522px |
| 14 | PREFOOTER | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 15 | FOOTER | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 336px → 593px |
| 16 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 214px → 593px |
| 17 | BLOG | 94 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px |
| 18 | GALLERY STYLES | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 685px → 1262px |
| 19 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 572px → 1262px |
| 20 | EVENT STYLES | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 609px → 1162px |
| 21 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 540px → 1162px |
| 22 | PRODUCT STYLES | 84 | Heading: proxima-nova 25px → Sofia Sans 25px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 536px → 1035px |
| 23 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 392px → 1035px |
| 24 | (no heading) | 97 | Text: adobe-garamond-pro 18px → EB Garamond 18px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.


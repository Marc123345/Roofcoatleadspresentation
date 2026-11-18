# RoofCoat Leads — pitch deck

A 16-slide sales deck for RoofCoat Leads, pitching lead generation to roof
coating contractors at $1,500 a month to us, plus about $50 a day of ad spend
paid by the contractor directly to Facebook. Revised 18 November 2026.

## Viewing it

Open `index.html` in a browser. Nothing to install and no network needed: the
fonts and photographs are embedded in the file, and the slide 9 ad videos sit
in `ads/`, so the folder works offline in a meeting room.

- Arrow keys, space or click to move between slides
- `F` for full screen
- Clicking the left third of a slide goes back

## Slides

| # | Slide |
|---|---|
| 1 | Title |
| 2 | What we do |
| 3 | The problem: a generalist agency learns your trade at your expense |
| 4 | Three ways contractors currently get work |
| 5 | Us against a generalist agency (head to head) |
| 6 | Why a specialist performs faster |
| 7 | Who this is for (and who it is not for) |
| 8 | Do you work with my competitor? |
| 9 | What the ads look like: the three video ads from roofcoatleads.com |
| 10 | What to expect: 20 to 50 inquiries a month per market |
| 11 | Results: lead-sheet inquiries by region, plus one contractor's $120,000 |
| 12 | The math: what one job covers |
| 13 | What $1,500 a month covers |
| 14 | How we work together after you sign |
| 15 | Month to month, no refunds, no guarantees |
| 16 | Pricing |

A winter slide for cold markets goes between 14 and 15 once the winter plan is
agreed with Ezra.

**Slide 9 videos** live in `ads/` next to `index.html` (same three ads as the
website's ad section, from ImageKit). They play muted on a loop while slide 9
is showing. The rest of the deck is still self-contained, but to show the ads
offline you need the `ads/` folder alongside `index.html`.

## Pre-call brief

`brief.html` is a separate one-page read for whoever is about to take the call —
not part of the 16-slide deck. It is the proof that already exists in the client
book: how many are paying, how many are under contract (none), who has stayed
longest, and the four stories that answer the objections contractors actually
raise.

Open it on its own. It prints to one page.

The counts come from the client record in `lib/clients.js` in the EZ Marketing
dashboard and were true on 8 September 2026. **Re-check them before a call if it
has been a few weeks** — the page says so at the foot. The four named stories
(Ron at Build Co, Pete Kelley, Byron, the Washington contractor) are Marc's own
account and are not recorded anywhere in code.

## Editing

The copy is plain HTML inside `index.html`, so text changes can be made
directly in that file. Search for the slide comments (`<!-- 12 . results`) to
find a slide.

`src/deck.template.html` is the same page with the embedded assets replaced by
placeholders (`__IMG_HERO__`, `__FONT_INTER__` and so on). It is far easier to
read and diff. Changing the template requires re-substituting the assets to
regenerate `index.html`.

## Numbers used

- **Lead-sheet figures on slide 11** (49 in 31 days Upper Midwest, 127 in three
  months Pennsylvania, 76 in five months Indiana, 22 in about a month Oklahoma
  and Arkansas, 2 commercial leads within 24 hours Idaho) are from the
  September 2026 lead sheets. Confirm before showing them by region.
- **$120,000 over three months against $9,000 paid** is one contractor's
  result, unnamed until he agrees to be named.
- **40% gross margin** on slide 12 is an assumption. "Months covered" there
  count fee plus ad spend, about $3,000 a month.
- The roof sizes and coating prices on slide 12 ($4 to $7 per square foot
  against $6 to $14 for a tear-off replacement) are industry ranges, not
  client results.

## Design

Built on the roofcoatleads.com design system: Montserrat and Inter, `#09090b`
ground, `#eab308` accent, with `#2563eb` as a secondary accent (the "from you" lists).

The deck stays dark whichever theme the viewer's browser is set to. That is
deliberate rather than an oversight: it matches the brand and it is what
projects properly in a room.

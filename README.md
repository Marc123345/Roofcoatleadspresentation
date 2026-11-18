# RoofCoat Leads — pitch deck

A 22-slide sales deck for RoofCoat Leads, pitching lead generation to roof
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

22 slides in four numbered sections. Each section opens with a divider
slide; every content slide carries a running section label top left.

| # | Slide |
|---|---|
| 1 | Title |
| 2 | What we do |
| 3 | Agenda (the four sections) |
| 4 | **Section 01: The problem** (divider) |
| 5 | A generalist agency learns your trade at your expense |
| 6 | Three ways contractors currently get work |
| 7 | Us against a generalist agency |
| 8 | **Section 02: Our approach** (divider) |
| 9 | Why a specialist performs faster |
| 10 | Who this is for |
| 11 | Do you work with my competitor? |
| 12 | The ads: three video ads, click to play (Facebook, Instagram, YouTube) |
| 13 | **Section 03: Results** (divider) |
| 14 | What to expect: 20 to 50 inquiries a month per market |
| 15 | Florida track record (287 inquiries, one contractor campaign) |
| 16 | The math: what one job covers |
| 17 | **Section 04: Working together** (divider) |
| 18 | What $1,500 a month covers |
| 19 | Sales and marketing: the gap every lead gen company has |
| 20 | How we work together (weekly calls, LeadConnector pipeline and notes) |
| 21 | Month to month, no refunds, no guarantees |
| 22 | Pricing |

A winter slide for cold markets goes between 20 and 21 once the winter plan is
agreed with Ezra.

**Slide 12 videos** live in `ads/` next to `index.html` (same three ads as the
website's ad section, from ImageKit). They play muted on a loop when clicked. The rest of the deck is still self-contained, but to show the ads
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

- **Florida figures on slide 11** come from one contractor's lead sheet:
  287 unique inquiries (repeats removed), 231 commercial and industrial (80%),
  56 residential, 136 cities and towns, 50 of 67 counties; top markets Miami
  20, Tampa 15, Orlando 13, Jacksonville 9, Fort Lauderdale 7, Ocala 7. The
  sheet has no dates, so the slide gives no time period. About 13% have
  incomplete or junk addresses, which is why the slide says "inquiries", never
  "qualified leads". Add "in X months" to the headline once the run length is
  known.
- The regional lead-sheet figures and the $120,000 story were taken off
  slide 11 on 18 November 2026 in favour of Florida.
- **40% gross margin** on slide 12 is an assumption. "Months covered" there
  count fee plus ad spend, about $3,000 a month.
- The roof sizes and coating prices on slide 12 ($4 to $7 per square foot
  against $6 to $14 for a tear-off replacement) are industry ranges, not
  client results.

## Design

Matches the roofcoatleads.com design system (`src/assets/css/rc.css` and
`style.css` in the roofcoat-leads repo): Beatrice Trial at weight 500 for
headings with the key phrase in gold, star-icon sub-titles, `#18181b` cards
with a 20px radius and a faded corner number, gold-edged highlight cards (dark,
white text, never solid yellow), a dashed gold callout, and photos as rounded cards. `#09090b`
ground, `#eab308` gold, no other accent colour.

Beatrice Trial has no punctuation glyphs, so `$ % , –` fall back to Inter
(embedded), the same way the site falls back to the system sans.

The deck stays dark whichever theme the viewer's browser is set to, to match
the brand and to project properly in a room.

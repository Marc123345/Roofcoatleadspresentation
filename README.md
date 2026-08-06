# RoofCoat Leads — pitch deck

A 16-slide sales deck for RoofCoat Leads, pitching lead generation to roof
coating contractors at $1,500/month plus $1,500 ad spend.

## Viewing it

Open `index.html` in a browser. Nothing to install and no network needed: the
fonts, logos and photographs are all embedded in the file, so it works offline
in a meeting room.

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
| 6 | What the campaigns are optimised for |
| 7 | The system: how the targeting improves |
| 8 | Why it compounds |
| 9 | Do you work with my competitor? |
| 10 | Who is on the system (logo wall) |
| 11 | Every contractor is month to month |
| 12 | Results: what one contractor did in three months |
| 13 | The cost of waiting |
| 14 | The math: what one job covers |
| 15 | What $1,500 a month covers |
| 16 | Pricing |

## Editing

The copy is plain HTML inside `index.html`, so text changes can be made
directly in that file. Search for the slide comments (`<!-- 12 . results`) to
find a slide.

`src/deck.template.html` is the same page with the embedded assets replaced by
placeholders (`__IMG_HERO__`, `__FONT_INTER__` and so on). It is far easier to
read and diff. Changing the template requires re-substituting the assets to
regenerate `index.html`.

## Numbers used

Two figures on the money slides are assumptions rather than measured values,
and both should be checked before presenting:

- **40% gross margin**, used on slide 12 to turn revenue into profit, and on
  slide 14 to work out how long one job covers the fee.
- **$100,000 in month one and $120,000 over three months** for the contractor
  on slide 12. Slide 13 extrapolates from that figure.

The roof sizes and coating prices on slide 14 ($4 to $7 per square foot against
$6 to $14 for a tear-off replacement) are industry ranges, not client results.

## Design

Built on the roofcoatleads.com design system: Montserrat and Inter, `#09090b`
ground, `#eab308` accent, with `#2563eb` reserved for the system diagram so the
mechanism reads differently from the money.

The deck stays dark whichever theme the viewer's browser is set to. That is
deliberate rather than an oversight: it matches the brand and it is what
projects properly in a room.

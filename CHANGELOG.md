# Changelog

## v1.5 (14 Nov 2026)
- **Reader's view:** text that is too big or too small looks wrong to the reader. On one page the same font now keeps one size: the median of the page, within ±5% (`pageBand`). Measured on Grimoire 12 page 05: Hayah sizes went from 0.84–1.54× to 0.84–1.05× of the median; size vs the editor's own finished pages 0.99× and 0.91×.
- Big bubbles get the page size with more air instead of huge text. A bubble too small for the page size keeps the SS margin (the text is never squeezed) and the log says "shorten the lines or add tatweel".

## v1.4 (14 Nov 2026)
- SS margin calibrated on real finished pages: the editor's side gap is about 1.1 em, while "سس" in Hayah measures 1.39 em, so the imagined letters count at 80% (`ssScale`). Top/bottom gap 15% of it (`ssVert`, was 50%).

## v1.3 (14 Nov 2026)
- **SS / سس rule:** the margin right and left of every line is the width of "SS" (English) or "سس" (Arabic) in the text's own font and size. BubbleFit measures it in Photoshop with a temporary text layer, then lets the text grow until those imagined letters reach the bubble edge, never touching it. Top and bottom gap: half of that width (`ssVert`).
- **Works with any active tool** (Magic Wand, Marquee, brushes...): it switches to the Move tool while it runs, then gives your tool and your layer selection back.

## v1.2 (13 Nov 2026)
- Keeps each text in the lobe it already sits in (joined bubbles, no RTL swap).
- Centres on the real ink: tatweel, hand-shaped lines and the text box size don't matter. Tashkeel above the first line or below the last line is ignored.

## v1.0
- First version: fits TypeR text into speech bubbles (Arabic + English), one Ctrl+Z undoes it.

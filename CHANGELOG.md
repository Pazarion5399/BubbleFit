# Changelog

## v1.3 (14 Nov 2026)
- **SS / سس rule:** the margin right and left of every line is the width of "SS" (English) or "سس" (Arabic) in the text's own font and size. BubbleFit measures it in Photoshop with a temporary text layer, then lets the text grow until those imagined letters reach the bubble edge, never touching it. Top and bottom gap: half of that width (`ssVert`).
- **Works with any active tool** (Magic Wand, Marquee, brushes...): it switches to the Move tool while it runs, then gives your tool and your layer selection back.

## v1.2 (13 Nov 2026)
- Keeps each text in the lobe it already sits in (joined bubbles, no RTL swap).
- Centres on the real ink: tatweel, hand-shaped lines and the text box size don't matter. Tashkeel above the first line or below the last line is ignored.

## v1.0
- First version: fits TypeR text into speech bubbles (Arabic + English), one Ctrl+Z undoes it.

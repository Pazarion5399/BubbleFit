# BubbleFit

A Photoshop 2025 script that fits your typeset text into its speech bubble, for Arabic and English. One Ctrl+Z undoes it.

## What it does
- Finds the bubble around each text and splits joined bubbles at their necks.
- **SS / سس rule:** imagine "SS" (English) or "سس" (Arabic), at the text's own size, right and left of every line. That gap is the margin to the bubble edge. BubbleFit fills the bubble right up to that margin: not smaller, never touching.
- **Reader's view (v1.5):** on one page the same font keeps one size (within ±5%). A big bubble gets the page size with more air, not huge text. A bubble too small for that size keeps the SS margin and is listed in the log: shorten the lines or add tatweel there.
- **Centring first (v1.6):** when a text is at its bubble's limit it keeps the largest size that fits exactly on the centre (giving up to 12% of size, `centreGive`) instead of sliding off-centre.
- Centres on the letters, not the tashkeel, and ignores the tail.
- Keeps your line breaks and shape (diamond / oval, tatweel): it only scales and moves the text.

## Video tutorial
BubbleFit v1.6 tutorial (55 s, English + Arabic): 3 steps, single and joined bubbles, the SS / سس rule, one size per page, always centred.

https://github.com/user-attachments/assets/f4641198-d303-462e-be8e-04128ac38129

(Can't play it? [Download the video](docs/video/BubbleFit_v1.6_tutorial.mp4).)

Older: [v1.3 tutorial](docs/video/BubbleFit_v1.3_tutorial.mp4).

## Use
1. Download `BubbleFit.psjs`.
2. Typeset with TypeR at a large size (over 75 px).
3. Select the text layers, or select none to fit the whole page.
4. Run File > Scripts > Browse > `BubbleFit.psjs`. Any tool can be active.

Settings are at the top of the `SETTINGS` block: `pageBand` (same size per page, ±5%; -1 = off), `ssRule`, `ssScale` (how much of the SS width counts, 0.8), `ssVert` (top/bottom gap, as a part of the SS width), `ssTouchEm`, `ssFill`, `maxScale`, `hardMin`.

## Licence
MIT - free to use, change and share.

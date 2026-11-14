# BubbleFit

A Photoshop 2025 script that fits your typeset text into its speech bubble, for Arabic and English. One Ctrl+Z undoes it.

## What it does
- Finds the bubble around each text and splits joined bubbles at their necks.
- **SS / سس rule:** imagine "SS" (English) or "سس" (Arabic), at the text's own size, right and left of every line. That gap is the margin to the bubble edge. BubbleFit fills the bubble right up to that margin: not smaller, never touching.
- Centres on the letters, not the tashkeel, and ignores the tail.
- Keeps your line breaks and shape (diamond / oval, tatweel): it only scales and moves the text.

## Use
1. Download `BubbleFit.psjs`.
2. Typeset with TypeR at a large size (over 75 px).
3. Select the text layers, or select none to fit the whole page.
4. Run File > Scripts > Browse > `BubbleFit.psjs`. Any tool can be active.

Settings are at the top of the `SETTINGS` block: `ssRule`, `ssVert` (top/bottom gap, as a part of the SS width), `ssTouchEm`, `ssFill`, `maxScale`, `hardMin`.

## Licence
MIT - free to use, change and share.

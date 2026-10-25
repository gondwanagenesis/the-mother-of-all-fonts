# The Mother of All Fonts

Free fonts made from the title cards of the 1968 Engelbart demo, plus a new lowercase, about a thousand symbols and 237 one-colour emoji drawn in the same hand.

Published by **The Swarm** under the **SIL Open Font License 1.1**. Use them for anything: install them, put them on websites and apps, print with them, change them, share them, ship them inside your own products. The one thing the license asks is that you don't sell the font files on their own, and that changed versions take a new name.

## The story

In December 1968, at the Fall Joint Computer Conference in San Francisco, Douglas Engelbart and his team from SRI's Augmentation Research Center gave a live demonstration to a hall of about 2,000 seats. In 90 minutes he showed a mouse, windows, hypertext links, editing on a shared screen and a video link to his lab in Menlo Park. It was later nicknamed "the mother of all demos."

The film of the demo opens with typed title cards. Every letter on them is drawn as a capital shape, and the real capitals wear a small bar above. That two-case trick is the starting point for this family.

## How it was made (October 2026)

- About 1,800 letters were cut from the title cards of the remastered video, lined up and averaged to wash out film grain, then traced to outlines.
- Q, Z, 1, 3, 4, 5, 7 and the letter I were not clear enough in the footage and were drawn by hand.
- Accented letters, punctuation, currency, math, arrows, shapes and box lines were then drawn to match: about 1,070 characters in each font.
- Humanist has a true lowercase. It is new work: the 1968 screen never had one.
- Spacing is optical, then tuned by eye on real paragraphs with about 80 hand-set kerning pairs. The Mono versions keep a fixed width for code and box drawing.

## The fonts

| Folder | Fonts | Use |
|---|---|---|
| `Fonts/` | AllCaps, SmallCaps, Humanist | Proportional and kerned, for text and titles. AllCaps: every letter a capital, real capitals carry a bar. SmallCaps: lowercase as shorter capitals. Humanist: true lowercase, the most readable. |
| `Fonts-Mono/` | the same three, "Mono" | Fixed width, for code and terminals. |
| `Fonts-Text/` | Humanist Text, SmallCaps Text (+ Mono) | A cut for sizes under about 16 px: stems about 35% heavier, taller x-height, looser spacing. See `small-size-comparison.png`. |
| `Emoji/` | NLS Display 1968 Emoji | The 237 emoji as a font of their own. |
| `Webfonts/` | every font as `.woff2` | For websites. |

## What is in each font

- All of ASCII: letters, digits and every keyboard symbol.
- Latin accents: all of Latin-1 and nearly all of Latin Extended-A (missing: ģ ĸ Ŀ ŀ ŉ ſ), so Western and Central European languages, the Baltics, Turkish and Welsh work. Vietnamese is almost complete. Also Ø, Æ, Œ, ß, Þ, Ð, Ł, Đ and a share of Latin Extended-B.
- Punctuation: curly quotes, « », dashes, ellipsis, bullets, dagger, section and pilcrow marks, inverted ! and ?.
- Money: $ ¢ £ ¤ ¥ € ₽ ₹ ₩ ₿. Math: ± × ÷ ≠ ≈ ≤ ≥ ≡ ∞ √ ∑ ∏ ∫ ∆ π.
- Fractions, superscripts and subscripts, © ® ™ ‰.
- Arrows, shapes, check and cross marks, card suits, music notes.
- Box-drawing lines, block and shade characters (best in the Mono fonts).
- 237 one-colour emoji (all the standard faces, plus hearts, hands, nature, animals, objects and symbols), built into every font.

Not included: Greek, Cyrillic, Arabic, Hebrew, Asian scripts, skin-tone and flag emoji. Capitals carry a bar, so an accented capital stands taller than the line: use line spacing of 1.3 or more with accents.

## Install

- **Windows:** select the `.ttf` files, right-click, choose *Install*.
- **Mac:** double-click a font, then *Install Font*.
- **Linux:** copy the `.ttf` files to `~/.local/share/fonts/` and run `fc-cache -f`.
- **Android:** apps that take a font file (Termux, launchers such as Lawnchair, Obsidian through a CSS snippet) can use them directly. Samsung and vivo phones only accept system fonts from their own theme stores.
- **Web:**

```css
@font-face {
  font-family: "NLS Display 1968 Humanist";
  src: url("NLS-Display-1968-Humanist.woff2") format("woff2");
  font-display: swap;
}
body { font-family: "NLS Display 1968 Humanist", system-ui, sans-serif; line-height: 1.4; }
```

The proportional, Mono and Text sets have different family names and will not clash.

## License

SIL Open Font License, Version 1.1. The full text is in `OFL.txt` and at <https://openfontlicense.org>. Free for personal and commercial use.

## Credits

Made by The Swarm, October 2026. Letterforms traced from the SRI International film of the 1968 demo, via the Doug Engelbart Institute's remastered video. This project is not affiliated with or endorsed by SRI International or the Doug Engelbart Institute. The film itself is not part of this package.
